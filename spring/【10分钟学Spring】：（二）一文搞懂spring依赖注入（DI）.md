Spring最基础的特性就是创建bean、管理bean之间的依赖关系。下面通过具体实例演示该如何装配我们应用中的bean。

### Spring提供了三种主要的装配机制
- 在xml中进行显示的配置
- 在Java中进行显示的配置
- 隐式的bean发现机制和自动装配

三种装配方式可依据个人喜好选择使用，无限制。不过应尽可能地使用自动转配机制，因为可以少一大推的配置。在你必须要使用显示配置时，比如要装配一些第三方的bean对象是，可以使用显示的配置。推荐使用类型安全且比xml更加强大的JavaConfig。

### 自动装配bean
1、创建bean并添加@Component注解

spring通过面向接口编程实现松耦合，因此平时在开发时要养成先创建接口，然后再实现类的习惯。
此处先创建一个CentralProcessUnit接口

```java
public interface CentralProcessUnit {
    void compute();
}
```
然后创建一个具体的实现类HisiCentralProcessUnit：

```java
@Component
public class HisiCentralProcessUnit implements CentralProcessUnit{
    public void compute() {
        System.out.println("海思芯片，计算。。。。。");
    }
}
```
可以看到，在该类上有一个注解@Component，表明该类是一个组件，spring在扫描的时候会自动创建该类的对象。

当然了，只添加这个注解是不够的。

2、开启组件扫描功能

为了能完成spring 的自动装配功能，除了在需要创建bean的类上添加@Component注解之外，还需要开启组件扫描功能。spring的组件扫描功能默认是关闭的。

开启组件扫描有两种方式：

- JavaConfig配置方式
-  xml配置方式

Java配置方式

```java
@Configuration
@ComponentScan
public class ScanConfig {
}
```
XML方式，在spring配置文件中增加如下这段就好：

```java
<context:component-scan base-package="com.herp"/>
```
3、新建测试类，验证bean是否注入

```java
@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(classes = ScanConfig.class)
public class AutoWiredBeanTest {

    @Autowired
    private CentralProcessUnit cpu;

    @Test
    public void testNotBeanNull(){
        Assert.assertNotNull(cpu);
    }
}
```
在该测试类中使用了@Autowired注解将扫描创建的bean对象注入到此测试类中。

通过上面的三个步骤我们可以看到，我们并没有使用new对象的方式，只是使用了一些spring的注解，spring便帮我们自动完成了对象的创建，并将其注入到了测试类中。

同样地，我们也可以在bean对象之间完成自动装配。我们再创建一个手机对象，然后将cpu芯片对象装配到手机对象中。

创建手机接口和实现类：

```java
@Component
public class HuaweiPhone implements IPhone{
    
    @Autowired
    private CentralProcessUnit cpu;
    
    public void compute() {
        cpu.compute();
    }
}
```
在HuaweiPhone 对象中自动装配CentralProcessUnit的实例。
**这里值得注意的是CentralProcessUnit是接口，如果有两个CentralProcessUnit实例，使用自动装配便会产生歧义性，因为spring容器不知道该装配哪个bean了。**

### 使用JavaConfig的显式配置
使用JavaConfig完成bean装配其实就是使用Java代码加spring的注解完成bean的配置、依赖的配置信息。

举例来说明：
本示例中，我们使用JavaConfig的方式完成CentralProcessUnit及IPhone实例的装配。

1、去掉HisiCentralProcessUnit 类上的@Component注解

```java
public class HisiCentralProcessUnit implements CentralProcessUnit {
    public void compute() {
        System.out.println("海思芯片，计算。。。。。");
    }
}
```

2、去掉ScanConfig中的@ComponentScan注解，只留下@Configuration注解，表示这是一个配置类。然后编写产生HisiCentralProcessUnit  bean的方法，并使用@Bean注解标注。

```java
@Configuration
public class ScanConfig {
    @Bean
    public CentralProcessUnit hisiCentralProcessUnit(){
        return new HisiCentralProcessUnit();
    }
}
```
3、如此便完成了最简单的bean的装配了。测试一下：

```java
public class JavaConfigWiredBeanTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(ScanConfig.class);
        HisiCentralProcessUnit cpu = applicationContext.getBean("hisiCentralProcessUnit", HisiCentralProcessUnit.class);
        cpu.compute();
    }
}
```
输出：

```java
海思芯片，计算。。。。。
```
可以看到完成了bean的转配。

4、同样地，我们去掉HuaweiPhone上的@Component注解，并提供一个带参数的构造器，注意参数类型是CentralProcessUnit（接口），而非具体实现类，具体类接下来我们会使用JavaConfig的配置的方式注入。

```java
public class HuaweiPhone implements IPhone {

    private CentralProcessUnit cpu;

    // 构造器注入
    public HuaweiPhone(CentralProcessUnit cpu){
        this.cpu = cpu;
    }

    public void compute() {
        System.out.println("华为手机+++");
        cpu.compute();
    }
}
```
5、我们在ScanConfig中加入huaweiPhone的配置，并注入hisiCentralProcessUnit实例。

```java
@Configuration
public class ScanConfig {

    @Bean
    public CentralProcessUnit hisiCentralProcessUnit(){
        return new HisiCentralProcessUnit();
    }

    @Bean
    public IPhone huaweiPhone(){
        return new HuaweiPhone(hisiCentralProcessUnit());
    }
}
```
6、验证依赖注入是否成功。使用AnnotationConfigApplicationContext容器类获取装配好的bean。

```java
public class JavaConfigWiredBeanTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(ScanConfig.class);
        // 依赖注入示例测试
        IPhone huaweiPhone = applicationContext.getBean("huaweiPhone",HuaweiPhone.class);
        huaweiPhone.compute();
    }
}
```
输出结果：

```java
华为手机+++
海思芯片，计算。。。。。
```

**使用JavaConfig配置bean和依赖关系，具有极大的灵活性，我们只需要在带有@Bean注解的方法上最终产生一个bean实例即可，具体bean实例的产生逻辑只受Java语言自身的限制。**

比如我们可以这样配置一个bean：

```java
    @Bean
    public CentralProcessUnit randomCentralProcessUnit(){
        int num = (int) Math.floor(Math.random() * 2);
        if(num == 0){
            return new HisiCentralProcessUnit();
        }else {
            return new GaoTongCentralProcessUnit();
        }
    }
```

这个CentralProcessUnit 是随机生成HisiCentralProcessUnit芯片或者是GaoTongCentralProcessUnit芯片。

### 使用XML完成bean装配和DI
XML配置的方式是spring最早采用的配置bean、bean之间的依赖关系的方式。

使用XML配置其实很简单，使用<bean>元素声明一个bean即可。

**1、最简单的bean配置**

```java
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="centralProcessUnit" class="com.herp.beanwired.xmlwired.GaoTongCentralProcessUnit"/>
</beans>
```
这样当spring发现<bean>元素时，会调用GaoTongCentralProcessUnit的默认构造器来创建bean。

**2、使用构造器依赖注入bean**

```java
    <bean id="iphone" class="com.herp.beanwired.xmlwired.HuaweiPhone">
        <constructor-arg ref="centralProcessUnit"/>
    </bean>

```

测试类

```java
public class XMLConfigWiredBeanTest {
    public static void main(String[] args) {
        ApplicationContext context = new ClassPathXmlApplicationContext("applicationContext-beans.xml");
        IPhone phone = context.getBean("iphone",IPhone.class);
        phone.compute();
    }
}
```
输出：

```java
华为手机+++
高通芯片，计算。。。。
```

3、使用属性注入bean依赖

```java
    <bean id="centralProcessUnit_hw" class="com.herp.beanwired.xmlwired.HisiCentralProcessUnit"/>
    <bean id="anotherPhone" class="com.herp.beanwired.xmlwired.HuaweiPhone">
        <property name="centralProcessUnit" ref="centralProcessUnit_hw"/>
    </bean>
```

同时，需要在HuaweiPhone类中提供setter方法

```java
    public void setCentralProcessUnit(CentralProcessUnit centralProcessUnit){
        this.centralProcessUnit = centralProcessUnit;
    }
```

测试类，替换成获取id为anotherPhone 的bean对象：

```java
public class XMLConfigWiredBeanTest {
    public static void main(String[] args) {
        ApplicationContext context = new ClassPathXmlApplicationContext("applicationContext-beans.xml");
        IPhone phone = context.getBean("anotherPhone",IPhone.class);
        phone.compute();
    }
}
```


输出如下：

```java
华为手机+++
海思芯片，计算。。。。。
```

### 总结
本节主要总结了spring装配bean和依赖注入的三种方式：组件扫描和自动装配、JavaConfig注解配置方式、XML配置方式。平时开发中优先使用组件扫描和spring自动发现的机制装配bean，这样可以省去大量配置类或配置文件，其次是使用JavaConfig的方式，一方面，它是类型安全的，另外在配置bean时提供了更大的灵活性。最后选用XML配置文件的方式装配bean。
