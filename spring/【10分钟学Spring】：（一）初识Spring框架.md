### 简介
Spring是一个轻量级的企业级的Java开发框架。主要是用来替代原来更加重量级的企业级Java技术，比如EJB(Enterprise JavaBean)、Java数据对象（Java Data Object）等。Spring的出现极大简化了Java开发。

另外Spring框架是一个一体化的框架，它不仅能无缝对接比如Struts、Hibernate等传统框架，也能很好地同其他各种企业级开发组件（比如Redis、MQ、Mybatis等）集成。

Spring发展到现在，已经不仅仅是一个开发框架了，而是一个生态。Spring框架本身提供了大量可集成到应用中组件，SpringBoot通过“约定优于配置的思想”进一步提高了开发效率，成为构建微服务应用的最佳选择，SpringCloud则提供了一套分布式工具组件，让构建分布式系统更加简单。

### Spring就是要简化Java开发
Spring一直致力于简化Java开发使命中，为了降低Java开发的复杂性，Spring通过如下4种关键策略来简化Java开发：

 - 基于POJO的轻量级和最小侵入性编程；
 - 通过依赖注入和面向接口编程实现松耦合；
 - 基于切面和惯例进行声明式编程；
 - 通过切面和模板减少样板式代码。

### Spring框架中的几个重要概念
**依赖注入（DI）**

对象之间的依赖关系，不再由对象自身来维护了。而是由spring负责管理了。依赖关系将会由spring负责自动注入到需要的对象中。

**切面编程（AOP）**

应用中的一些横切关注点，比如日志、安全、事务管理等，各个模块都需要的服务，不应该耦合在各个业务模块中来。应该单独抽离出来成为一个切面，实现解耦。Spring提供了AOP的支持，可以通过配置实现切面编程。

**Ioc容器（ApplicationContext）**

在基于Spring的应用中，你的所有Bean对象都存在于Spring容器中，容器负责创建和管理他们的整个生命周期。ApplicationContext应用上下文对象是Spring容器的一种实现。通过应用上下文对象我们可以获取应用中bean。

### Spring模块概述
一图胜千言

![在这里插入图片描述](https://img-blog.csdnimg.cn/20191204223212908.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L20wXzM3OTY1MDE4,size_16,color_FFFFFF,t_70)
可以看到spring其实包含了20多个不同的模块。

1、spring核心容器，包含四大模块，分别是Beans、Core、Context和SpEL。这是构成spring框架的核心组件。

2、再网上是AOP、Aspects切面编程相关组件，Instrunmentation是JVM添加代理，Messaging消息代理。

3、JDBC、ORM、JMS等数据访问组件。

4、Servlet、WebScoket等web层相关组件。

5、最后spring也提供了测试模块，可以集成Junit单元测试等。

### 推荐几个Spring学习途径

**1、 当然优先是spring官网，查看官方文档学习**
 
![在这里插入图片描述](https://img-blog.csdnimg.cn/20191204224235668.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L20wXzM3OTY1MDE4,size_16,color_FFFFFF,t_70)

**2、W3Cschool**

![https://www.w3cschool.cn/wkspring/](https://img-blog.csdnimg.cn/20191204224429520.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L20wXzM3OTY1MDE4,size_16,color_FFFFFF,t_70)
**3、CSDN或博客园等技术文章**
