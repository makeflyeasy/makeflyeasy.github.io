### <center>Pixhawk航测固定翼自学笔记<center>
<div align='center' ><font size='5'>前言</font></div>
  
&emsp;&emsp;3年多以前，因为买不起昂贵的商业飞控，开始了对Pixhawk飞控用于航测的探索，经过几千个架次的实际飞行，Pixhawk还是非常稳定的。每次有朋友问这个Pixhawk飞控是怎么调试的，只能零零散散地回答一些，网上也有相关教程，但对于Pixhawk在航测固定翼上的使用不是很全面，这就是我把学习笔记公布出来的原因。  
&emsp;&emsp;自学笔记主要参考官网的教程和自己的实际使用经验总结而来，因为个人的知识面有限，笔记难免有不全或者错误的地方，请大家指正，我会及时修正。  
&emsp;&emsp;我希望这个学习笔记  
&emsp;&emsp;能帮助到无人机相关专业的学生，学习理论知识同时，实践组装一台低成本航测固定翼；  
&emsp;&emsp;能帮助到航模转航测的朋友，早点体验自动驾驶的乐趣；  
&emsp;&emsp;能帮助到航拍转航测的朋友，固定翼也能和多旋翼一样简单；  
&emsp;&emsp;能帮助到油动转电动的朋友，电动固也能干油动固定翼的项目；  
&emsp;&emsp;能帮助到测绘行业里不懂航测固定翼的新人，能够快速上手航测业务；  
&emsp;&emsp;我想这就是makeflyeasy航测存在的意义！  
&emsp;&emsp;吃水不忘挖井人，感谢ArduPilot这个伟大的开源组织持续不断地升级固件免费让我们用；感谢伟大的时代，让我们在神奇的国度里可以低成本地一站式采购完所有零件；感谢同事的理解和支持，帮助我尽可能详细地把这本书写完；感谢家人的宽容、陪伴、I LOVE YOU！  
<p align="right">
Makeflyeasy
<p align="right">
20180830

### 1 空机组装
#### 1.1一览全局
&emsp;&emsp;空机的组装采用信仰者1代航测载机，信仰者1代的最大的优点是：方便拆装、方便携带，最大的缺点是：手动起飞困难，对操作手的要求比较高。为了避开手动起飞，在航测作业中，我一般使用自动起飞，手动开伞的方式降落。  
![0.jpg](https://i.loli.net/2021/01/23/E8hjp39aWZDQrPe.jpg)
&emsp;&emsp;现售的包装里面增加了EPS保护泡沫，适合长期运输使用，箱子的大小可以放在普通的小汽车后备箱中，还是比较方便。  
![1.jpg](https://i.loli.net/2021/01/23/f73d8JoODpm1eWT.jpg)
&emsp;&emsp;整个机体的EPO材料还是偏软，主要是EPO的厚度不够，整个EPO拿在手里很轻，缺乏厚重感和工程测量装备的皮实感。但是作为一款入门级的航测载机，已经够用了，机体还是比较宽阔，方便安装设备，无工具拆装和便携的特点，用起来还是很顺手。  
![2.jpg](https://i.loli.net/2021/01/23/1vfqikyw8zuP9Se.jpg)
&emsp;&emsp;配件很多，增加了组装的复杂度，但是为了使用方便，这一切都是有必要的。建议装之前一定要看一遍说明书，避免错装和漏装。  
![82.jpg](https://i.loli.net/2021/01/23/VXuo2OvLxtZsFIC.jpg)
&emsp;&emsp;装好以后，为了增加机翼尾翼的强度，建议舵面用纤维胶带加强，飞行的品质可以得到提升。  
#### 1.2机翼尾翼部分
&emsp;&emsp;先从机翼开始装，电机座的泡沫槽里面一定要涂满泡沫胶，最好把电机座用热熔胶固定，避免在降落过程中，桨扫地引起的电机座松动，在起飞前务必检查电机座是否有松动。
![8.jpg](https://i.loli.net/2021/01/23/hQNeRsm3YV4vZCM.jpg)
合上机翼盖板，一定要压紧、对齐，安装塑料螺柱
![16.jpg](https://i.loli.net/2021/01/23/4v5YBLsQygRClWJ.jpg)

安装舵机槽的时候，一定要注意舵机线的出口方向
![19.jpg](https://i.loli.net/2021/01/23/ZJV3OLYxDjh8qBn.jpg)
机翼翼根塑料件涂泡沫胶时候不要弄到碳管洞里面了，不然后面拔插碳管会很紧
![25.jpg](https://i.loli.net/2021/01/23/KMZnDqv1TBCGals.jpg)
尾翼为了防止碳管松动，在碳管接缝处涂满泡沫胶固定
![32.jpg](https://i.loli.net/2021/01/23/HXUiwDy9O8MhFaN.jpg)
接触面涂胶后，合上尾翼塑料件，尾翼就组装完成了
![33.jpg](https://i.loli.net/2021/01/23/fE6COrtoMjbpAgL.jpg)
#### 1.3机身部分  
机身合模之前需要提前预装机身主副碳管、机身木板加强件
![45.jpg](https://i.loli.net/2021/01/23/lj31IVDFPNArEWe.jpg)
尾翼木板加强件也需要预装
![47.jpg](https://i.loli.net/2021/01/23/bstaDYWvRqGjPfi.jpg)
机身中端的耐力板和机头的耐力板也需要预装
![54.jpg](https://i.loli.net/2021/01/23/Q4hkP1KFlbwCoJM.jpg)
![55.jpg](https://i.loli.net/2021/01/23/UbruhinMOlydBXm.jpg)

装好以后，就可以根据机身结合部分开始涂胶了
![56.jpg](https://i.loli.net/2021/01/23/5qAHnrB1R46vu9L.jpg)
涂完胶以后一定要对齐、压紧、合实
![57.jpg](https://i.loli.net/2021/01/23/QiOTXPfZJ8uSgrj.jpg)
接下来安装机身翼根塑胶件
![60.jpg](https://i.loli.net/2021/01/23/yY4KGNhJvRBdQfA.jpg)
尾翼翼根塑料件
![61.jpg](https://i.loli.net/2021/01/23/pzq3StTQsPRdaX9.jpg)
#### 1.4小零件部分

先安装伞舱舵机固定木板
![69.jpg](https://i.loli.net/2021/01/23/z3w9WHkxRbGi1lX.jpg)
接下来，粘合伞舱盖、飞控舱盖、电池舱盖等
![38.jpg](https://i.loli.net/2021/01/23/ZIyDM8LzKdmUWHj.jpg)
![41.jpg](https://i.loli.net/2021/01/23/RsUF5HT6tDVQcP3.jpg)
![42.jpg](https://i.loli.net/2021/01/23/A4WKJTgEDvkoaYj.jpg)


粘合电池固定板，注意电池板的方向，两边不是对称的，只有一个方向可以和泡沫紧密贴合。
![65.jpg](https://i.loli.net/2021/01/23/hqJdrZVQMFKY9UT.jpg)

粘上耐磨垫，一定要压实，缓解降落的冲击力
![72.jpg](https://i.loli.net/2021/01/23/TsogGLdbASPepEr.jpg)
插上电池舱、飞控舱、图传舱的锁扣
![79.jpg](https://i.loli.net/2021/01/23/t1RxC6iKT5HsVOP.jpg)
到这里整个空机的组装部分就完成了。  
### 2 Pixhawk2.4.6飞控调试
#### 2.1地面站安装
地面站的安装我使用的是mission planer 1.3.58，  
官方下载地址：
[mission planer 1.3.58](http://firmware.ap.ardupilot.org/Tools/MissionPlanner/ )  
安装过程中出现360拦截，一定要关掉，点击下一步  
![2.1.1.jpg](https://i.loli.net/2021/01/23/VrGDYU74pMIEv5H.jpg)  
配置安装路径，开始安装
![2.1.2.jpg](https://i.loli.net/2021/01/23/LBKpXTGYIivRnW6.jpg)  
安装完成后，一定要接上飞控，检查驱动是否安装成功
![2.1.3.jpg](https://i.loli.net/2021/01/23/lLQaREDKpiWM1PJ.jpg)
![2.1.5.jpg](https://i.loli.net/2021/01/23/sAwkPcft2Vh9zJp.jpg)
如果未能安装成功，找到MISSION PLANER的安装目录，手动更新驱动
![2.1.6.jpg](https://i.loli.net/2021/01/23/3hkUzubMp5WT19Z.jpg)
#### 2.2给飞控刷固件
&emsp;&emsp;目前PXIHAWK的改版比较多，我建议使用2.4.6原版 ，2.4.8属于2.4.6的阉割版，为了降低成本删除了电源3度冗余设计。其他版本在使用之前一定要了解清楚提升了哪些性能，删除或者简化了哪些接口和功能，谨慎使用。

&emsp;&emsp;给飞控刷固件之前，一定要准备一根好的USB数据线，因为数据线太差，电压压降太大，会引起飞控异常，一定要准备一张正版的高速MICRO SD卡，避免飞控日志写入出现异常（淘宝上买的飞控自带的卡很容易出问题，卖家为节约成本一般用低端卡）。
![2.2.1.jpg](https://i.loli.net/2021/01/23/i9yEqQX4uVSWN3z.jpg)
刷固件之前，一定要插入SD卡，否则固件刷不进去  
打开Mission Planer,找到正确的串口号，波特率为115200，在初始设置一栏中，找到安装固件，点击ArduPlane V3.9.0下载固件即可  
![2.2.2.jpg](https://i.loli.net/2021/01/23/1AB8IqnUdgE9Kb7.jpg)
注意：目前ChibiOS版本支持得还不是很完善，目前阶段建议选择No
![2.2.3.jpg](https://i.loli.net/2021/01/23/dZrPbuJ5j2qHtvF.jpg)
上传完以后，点击链接，就可以看到飞控的版本信息
![2.2.4.jpg](https://i.loli.net/2021/01/23/nwGJrgZsX4IzcL6.jpg)
这样固件就上传成功了
#### 2.3 GPS连接检查
&emsp;&emsp;GPS我使用的UBLOX NEO M8N模块，可以满足一般的导航需求，我没有使用外置电子罗盘功能，所以没接线，实际使用中也没用内置罗盘，我把罗盘功能禁用了。罗盘容易被干扰，注意事项很多，飞机容易出现一些莫名其妙的异常。
![2.3.1.jpg](https://i.loli.net/2021/01/23/BahkDgz5R82FwCX.jpg)
我们的GPS配置的串口3，飞控可以自动匹配GPS，所以只需要把线接对就行。
![2.3.2.jpg](https://i.loli.net/2021/01/23/rLupFevCZdwQVls.jpg)
&emsp;&emsp;我飞控通电后，把GPS拿到户外搜星，室内一般要等很久才能搜到，搜到星的时候，GPS的指示灯开始闪烁，表示GPS开始定位了。
为了省事，我用充电宝连接飞控，把GPS拿到屋外搜到星，等到GPS的指示灯闪烁后，再拿到室内用USB连接地面站检查。
![2.3.3.jpg](https://i.loli.net/2021/01/23/Oz5ni7G8FaCJmoK.jpg)
通过地面站，可以看到GPS得噪声和搜星数量，在左下方的参数栏也可以看到搜星情况，注意GPS状态3是GPS3D定位的意思。
![2.3.4.jpg](https://i.loli.net/2021/01/23/oOpb7v1U23adiWV.jpg)
虽然信号不是很多，但是GPS模块的整个功能都是正常的，拿到室外长时间搜星，卫星一般在20颗左右。
#### 2.4 电流电压检测模块连接配置
&emsp;&emsp;电压检测模块，不仅可以检测流入的电压和电流，还提供了5.3V@3A的电源给飞控供电，这个电源非常重要，飞控供电主要靠它。
![2.4.1.jpg](https://i.loli.net/2021/01/23/eEWwGyzm4ax7Ksk.jpg)
在全部参数列表里面开始电池参数配置
![2.4.2.jpg](https://i.loli.net/2021/01/23/YoxOaKgFrn6XAp9.jpg)
BATT_AMP_PERVLT配置为17，电流检测模块每输出1V的检测电压对应的电流为17A。  
BATT_CAPACITY配置为16000，一般使用的是6S16000mah电池  
BATT_CURR_PIN配置为3，PIXHAWK飞控所对应的电流检测引脚  
BATT_MONITOR配置为4，电流和电压都要检测  
BATT_VOLT_MULT配置为10左右（后面讲电压校准），电压检测模块每输出1V所对应的电压。  
BATT_VOLT_PIN配置为2，PIXHAWK飞控所对应的电压检测引脚  
配置完成后，重启飞控  
电流电压的校准的方法  
![2.4.3.jpg](https://i.loli.net/2021/01/23/mNFf72jgnusEOYR.jpg)

#### 2.5 蜂鸣器的连接配置
&emsp;&emsp;蜂鸣器主要是表示飞控的一些状态，不同的状态声音不一样，我不太擅长听声音，具体什么声音代表什么含义，官网有详细的介绍  
[蜂鸣器声音含义链接](http://ardupilot.org/plane/docs/common-sounds-pixhawkpx4.html#common-sounds-pixhawkpx4)  
蜂鸣器的接线图如下  
![2.5.1.jpg](https://i.loli.net/2021/01/23/OngGYaf5bv4U7uM.jpg)
蜂鸣器是靠振动发出声音的，所以为了防止蜂鸣器干扰加速度计，一般蜂鸣器至少远离飞控5CM
#### 2.6 安全开关的连接配置
安全开关主要用于开启或者关断电机和舵机的信号输出
![2.6.1.jpg](https://i.loli.net/2021/01/23/bf23Q5CWvF4uj97.jpg)
安全开关上灯的含义：  
LED持续闪烁-系统正在初始化；  
LED间歇性闪烁-系统准备好了，按下安全开关电机舵机信号输出；  
LED固体-安全开关已按下，电机和舵机能够正常输出信号；  
配置安全开关  
BRD_SAFETYENABLE配置为1，启用安全开关功能；配置为0关断安全开关功能；  
![2.6.2.jpg](https://i.loli.net/2021/01/23/qLWJGtOZEHnSVpj.jpg)
#### 2.7 飞控调试—LED灯的含义与配置
这里的LED指的是飞控上的三色LED，不同的颜色和闪烁代表不同的含义
下面列出常见的LED灯显示情况：  
&emsp;&emsp;蓝灯闪烁：飞控已解锁，但是GPS没定位，飞控盘旋模式和返航模式需要GPS定位；  
&emsp;&emsp;蓝灯固定：飞控锁定，但是GPS没定位；  
&emsp;&emsp;绿灯闪烁：飞控准备上锁，GPS已经定位；上锁时有快速的双响  
&emsp;&emsp;绿灯快闪：飞控已解锁，GPS已经定位，GPS使用的是SBAS(所以应该有更好的位置估	计)  
&emsp;&emsp;绿灯固定伴随着一声解锁长音：飞控解锁，GPS已经定位，准备起飞  
&emsp;&emsp;双闪黄灯：飞行前检查失败，飞控拒接解锁  
&emsp;&emsp;单黄灯闪烁：遥控器接收机没有信号  
配置LED的亮度  
<font color='red'> 注意：USB供电LED的亮度变化感觉不出来，接上飞控电源供电，可以感受到明显变化 </font>  
![2.7.1.jpg](https://i.loli.net/2021/01/23/Kks7WNaq3vIPnUz.jpg)
默认为高最亮
#### 2.8 空速计连接配置
&emsp;&emsp;空速计主要测量飞机的空速，我使用的MS4525D0这款，I2C接口，抗干扰性比模拟的要好一些。空速计的I2C接口接飞控的I2C口就行了。空速计上面有两根管，上面的是动压管，下面的是静压管，一般下管直接在飞机内部不接，上管接空速计管延伸到机身外。
![2.3.1.jpg](https://i.loli.net/2021/01/23/35CMfQp1Fuh6Nlc.jpg)
我们目前使用单空速计，地面站的配置如下
![2.3.2.jpg](https://i.loli.net/2021/01/23/DIHX9nk3wpeqjQu.jpg)
ARSPD_BUS配置为0，使用内部的I2C 0  
ARSPD_SKIP_CAL配置为0，每次重启飞控，需要校准空速计偏移，需要每次把空速帽子带上；  
设置为1，自动跳过空速偏移校准，使用上次校准的偏移量。一般长期飞的话，只在飞控出现异常才校准偏移，不用每次校准，太麻烦了。  
ARSPD_TUBE_ORDER配置为2 自动匹配上管或者下管为动压，简单地说你不管怎么接都不会错。  
ARSPD_TYPE配置为1，使用的是1:I2C-MS4525D0   
配置完成以后，一定要重启飞控，空速计才会生效  
在地面站的调试界面里面，观察空速计的变化，一般数值跳动在1-3以内都是正常的。  
向空速计里面吹气，如果空速增加，说明空速计工作正常。  
![2.3.3.jpg](https://i.loli.net/2021/01/23/EJGZCduehpF9xsi.jpg)
&emsp;&emsp;如果空速计数值太大没在正常的范围内，就需要校准空速计，正常的校准步骤：找到“动作”界面开面有“PREFLIGHT_CALIBRATE”，点击“执行动作”就可以了。（校准空速的动压管一般是在没风条件下进行，没得这样条件，用物体密封一下创造条件）。
![2.3.4.jpg](https://i.loli.net/2021/01/23/szux8PGCA5gE4Mc.jpg)
配置巡航空速
![2.3.5.jpg](https://i.loli.net/2021/01/23/vcMgK2FrRftCyT5.jpg)
TRIM_ARSPD_CM注意这个参数修改以后，必须要重启飞控才会生效。
### 3 动力系统调试
#### 3.1电机电调的连接与测试
&emsp;&emsp;电机采用的2820KV550型号，配APC1170桨单个推力在2.8KG左右，配APC1260桨，单个推力在3.5KG左右，目前用得最多的还是1170的桨，主要是滑降的时候，桨不扫地。  
&emsp;&emsp;电机在机翼安装的时候，一般使用外转，增强飞机的安定性（电机外转指旋转方向朝外）。  
&emsp;&emsp;任意改变电机3根线的2根，可以改变电机的转向。  
![3.1.1.jpg](https://i.loli.net/2021/01/23/kTqYeo8HVhB6JEP.jpg)
&emsp;&emsp;使用舵机测试仪，可以检测电机、电调是否正常工作，舵机测试仪需要单独的5V供电
![3.1.2.jpg](https://i.loli.net/2021/01/23/rVhKLJAw6n2SXgY.jpg)
&emsp;&emsp;电调的油门行程校准方法：在通电之前把舵机测试仪旋钮拧到最大输出，接通电源，听到滴滴声音，再把舵机测试仪的旋钮拧到最小输出，听到一声长滴，表示校准成功。  
&emsp;&emsp;电调最好使用不带BEC功能的，因为电调里面的BEC大多采用线性稳压，发热量很大，影响电调的正常使用功能，容易烧。  
&emsp;&emsp;有条件的情况下，把电机、电调、桨放在拉力测试仪上检测电机的工作效率，电机的骤起骤停有无异常，电调长时间工作发热是否异常等。  
![3.1.3.jpg](https://i.loli.net/2021/01/23/SKbne3acNisMg9T.jpg)
#### 3.2 BEC5V-10A的检测
&emsp;&emsp;BEC5V-10A的电源模块，主要是给舵机供电，不要把数传供电也接在这个电源上，因为舵机里面的电机在工作过程中会引起电压波动比较大，RDF900数传模块里面是LDO供电，允许的电压不是很大，容易被烧。  
&emsp;&emsp;为了确保BEC5V-10A电源模块的可靠性，我用电子负载进行了实际测量，主要测量两个指标，10A的恒定输出，和5-10A跳变输出测试，发热情况在可接受范围以内。  
&emsp;&emsp;实际工作中，舵机没有这么大的工作电流，我在电源模块的选择上面，一般是3倍冗余。 
![3.2.1.jpg](https://i.loli.net/2021/01/23/um71NwzD5f9TLHs.jpg)
&emsp;&emsp;BEC5V-10A的电源模块需要把舵机的+和-分别并联在一起，在飞控上的舵机电调接线口的+和-都是分别并联在一起的，所以BEC5V-10A电源模块只需要接一个闲置口，就可以给所有的舵机供电。
![3.2.2.jpg](https://i.loli.net/2021/01/23/o3iurUw8Bec2OsC.jpg)
#### 3.3 BEC5V或12V-3A调压与检测
BEC5V-3A主要是给数传独立供电，BEC12V-3A可以给A7R假电池供电、或者给差分GPS供电。
![3.3.1.jpg](https://i.loli.net/2021/01/23/R4fod2hlkzHQpcx.jpg)
输入端接上电池，输出端接上万用表，旋转调压按钮到所需要的电压。
#### 3.4 动力系统调试—舵机检测与摇臂归置中位
一般使用舵机测试仪检测舵机是否正常，舵机测试仪需要BEC单独供电。
![3.4.1.jpg](https://i.loli.net/2021/01/23/42NtDrbIn8eaAKm.jpg)
把舵机测试仪调到手动挡，拧旋钮，观察舵机摆动情况，舵机有无异响和抖舵现象。  
把舵机测试仪调到归中挡，此时舵机左右两边的行程一样大。  
把舵机测试仪调到自动挡，按照说明书的扭力值，给舵机摇臂挂上匹配的重物，舵机来回摆动，这样可以测试舵机的使用寿命，对舵机选型提供参考依据。  
#### 3.5 电池的放电区间与电显的使用
&emsp;&emsp;我一般使用6S 16000mah的锂聚合物电池，放电系数25C，电池尺寸66*74*185mm,重量1800g，接头使用XT90防打火。
![3.5.1.jpg](https://i.loli.net/2021/01/23/Lo9BAklMKENHZRd.jpg)

&emsp;&emsp;一般锂聚合物电池充电截止电压4.2V,放电截止电压3.7V，充放电次数在200次左右，需要专门的平衡充电器进行充电。  
&emsp;&emsp;电池电压低于3.7V，余电不是很多，长期使用会加速电池老化，一般使用电量显示器检测检测电池电压，6S电池充满电压25.2V，放电截止电压22.2V
![3.5.2.jpg](https://i.loli.net/2021/01/23/wyt2lgKbJu7QXnx.jpg)
#### 3.6 电源分电盘的焊接与接线图
&emsp;&emsp;需要供电的设备比较多，电源为了方便连接，使用了分电盘，分电盘才有2盎司铜厚的，保证过流能力，电池输入端采用12AWG硅胶线，尽可能减小压降。
![3.6.1.jpg](https://i.loli.net/2021/01/23/cG6IuCbnzrtADLN.jpg)
&emsp;&emsp;有条件的情况下，可以把需要供电设备的电源线直接连在一起，不使用分电盘，减小分电盘发热和损坏的概率。  
&emsp;&emsp;整个飞机的主电源接线图如下：
![3.6.2.jpg](https://i.loli.net/2021/01/23/fO2lxEIjtwLJZdX.jpg)
### 4. 遥控系统调试
#### 4.1 遥控器的介绍与设置
遥控器采用天地飞7，一共有7个通道。  
同时按住menu键和开机键，进入系统设置。  
在机型设置中为固定翼  
有可以配制教练/模拟器模式（一般就选普通模式）  
供电方案设置为锂电  
设置完成后，需要重新开机（不再需要按menu键了）  
![4.1.1.jpg](https://i.loli.net/2021/01/23/PGMbOw7u5BQzsyl.jpg)
#### 4.2接受机LED灯含义与对码
&emsp;&emsp;接收机支持宽电压输入，我一般接5V，一般配置到WBUS模式（默认就是WBUS模式，WBUS和SBUS的协议是一样的，只是厂家换了一个名称而已）
![4.2.1.jpg](https://i.loli.net/2021/01/23/6UwkiGnMAh42e7y.jpg)
和飞控的接线一定要接对，是接RCIN口  
![4.2.2.jpg](https://i.loli.net/2021/01/23/pX7gUlbKjzcQ32e.jpg)
遥控器对码的步骤：    
&emsp;&emsp;打开遥控器，按menu键，找到“高级设置”一栏，点击“ENTER”，找到“对码”一栏，再点击“ENTER”，接下来长按接受机上的SET 3秒，进入对码，黄灯慢闪。    
&emsp;&emsp;对码成功后，接收机上指示灯为绿色。  
![4.2.3.jpg](https://i.loli.net/2021/01/23/Yd542fmikwIAu1R.jpg)
#### 4.3 遥控器锂电池供电模式的设置及充电注意事项
用锂电池给遥控器供电时，在遥控器配置里面，配置到锂电池模式，其他电池的电压太低很快容易报警。
![4.3.1.jpg](https://i.loli.net/2021/01/23/TuCIHprD1vnl9XV.jpg)
锂电池一般的充满电压为4.2V，放电截止电压3.7V，一定要用专门的充电器充电。
![4.3.2.jpg](https://i.loli.net/2021/01/23/1BqKeLyouOw4xCU.jpg)
#### 4.4遥控模拟器的安装与加密狗配置
准备好加密狗、转接线、延长线、一端连接到遥控器，USB端连接到电脑
![4.4.1.jpg](https://i.loli.net/2021/01/23/nJckKzgduBIAUN6.jpg)
遥控器设置为模拟器模式
![4.4.2.jpg](https://i.loli.net/2021/01/23/scpYHXE34AIQZFv.jpg)
安装模拟器
![4.4.3.jpg](https://i.loli.net/2021/01/23/jfCEhu4XR1LyATo.jpg)
安装成功后，点击控制台切换模式
![4.4.4.jpg](https://i.loli.net/2021/01/23/hbwUQHp8SyEmJnd.jpg)  
安装完凤凰模拟器以后就可以打开软件看到这个界面
![4.4.5.jpg](https://i.loli.net/2021/01/23/FhNj1tYJgxly2sB.jpg)

#### 4.5 模拟器的配置
先配置遥控器
![4.5.1.jpg](https://i.loli.net/2021/01/23/4smg8vODV3T5Ftz.jpg)
接下来按照向导配置遥控器
![4.5.2.jpg](https://i.loli.net/2021/01/23/8aRjJ2XyNVShUBb.jpg)
检查通道配置是否正确
![4.5.3.jpg](https://i.loli.net/2021/01/23/BTpDm2w3v7Fb5fX.jpg)
接下来就可以开始练习了
#### 4.6 模拟器的起降训练心得
在选择模型里面，选择上单翼的飞机，飞机比较稳定，好飞。
![4.6.1.jpg](https://i.loli.net/2021/01/23/gwz3Pqe8bVWEnv9.jpg)
场地选择有明显跑道的，这样可以对着跑道练习起降
![4.6.2.jpg](https://i.loli.net/2021/01/23/zYlSAMLgfrds6vc.jpg)

快速上手飞机方法：  
1.飞机上天后尽量保持飞机高度不变，飞矩形航线，增强对飞机的操作手感。  
2.练习飞机起降，要求降落远距离对跑道、降落平稳、飞机不跳。  
有空要勤加练习，不要随意飞，每次给自己定个小目标，为实际飞行打下基础。  
![4.6.3.jpg](https://i.loli.net/2021/01/23/BpbdnFES6IhuAjG.jpg)

### 5 数传系统调试
#### 5.1 RDF900数传功能及引脚介绍
RDF900是一款不错的数传，天线配置合理以后，正常平原通信距离10KM以上，天空端和地面端的模块是相同的。  
![5.1.1.jpg](https://i.loli.net/2021/01/23/sQb4wq2ZdxpWviI.jpg)
我们只需要连接+5V 、GND、SIRX、SITX这四个引脚就可以了，以其他的现在用不上。  
地面通过USB转串口模块连接数传，注意串口的RX接数传的TX，数传的RX接串口的TX，弄错了连不上。  
数传的天空端直接连飞控就可以的，同样是飞控的RX接数传的TX，飞控的RX接串口的TX，弄错了连不上，但是不会烧坏。  
![5.1.2.png](https://i.loli.net/2021/01/23/4iamDbdCA5yMWLw.png)
#### 5.2 天空端胶棒天线特点与延长线
天空端天线增益5dbi  
增益：5dbi± 0.7dbi  
驻波比：<= 1.8  
阻抗：50ohm  
接头型号：SMA内螺纹内孔  
总长：19.5CM  
![5.2.1.jpg](https://i.loli.net/2021/01/23/lkGLeZHmSiKWqI4.jpg)
#### 5.3 天空端PCB天线特点与注意事项
PCB天线尺寸比较小，适合放在机身内部  
频率范围：800~2170 MHz   
增益：5dbi± 0.7dbi  
驻波比：<= 2.0  
阻抗：50ohm  
天线尺寸:125mm*14mm*0.8mm  
馈线长55cm,接头为SMA内螺纹内孔  
![5.3.1.jpg](https://i.loli.net/2021/01/23/Lws6T1PnGB8JSqW.jpg)
#### 5.4 地面端高增益天线的特点与注意事项
地面端天线参数：  
天线高度:72CM  
直杆接口类型:UHF公头  
底座直径:9cm  
底座接口类型:UHF母头  
馈线长度:3米  
接头类型:SMA内螺纹内孔  
频率:900MHz  
增益:38dBi  
![5.4.1.jpg](https://i.loli.net/2021/01/23/kc9RKxysDPZ74f1.jpg)

#### 5.5 RDF900地面站配置参数方法
用USB转串口连接数传，打开地面站，选对串口号，波特率设置为57600，  
数传上灯的含义：  
绿灯闪烁，表示正在对码  
绿灯常亮，表示数传对码成功  
红色闪烁，表示数据在通信  
绿灯常亮红灯不亮—一般是数传的TX/RX接反了  
![5.5.1.jpg](https://i.loli.net/2021/01/23/PupYoHUQIZ5wMc9.jpg)
&emsp;&emsp;连上地面站以后，可以看到数传的参数，一般默认发货的时候，数传是配置OK的。  
如果有多对数传同时工作，可以修改数传的ID号，让不同ID号的数传对，分别工作。  
为了获得更远的距离，可以调整发射功率，设置为30DB（1W）  
&emsp;&emsp;配合这一套数传模块、天线在丘陵地区一般10KM以上没得什么问题，因为我的数传从来没断过，最大能飞多远，可以期待！  
### 6 影像系统调试
#### 6.1 相机参数的配置与注意事项
&emsp;&emsp;目前正摄影用得最多的相机是A7R，配合35mm镜头，全画幅微单3600W像素，传感器尺寸35.9mm*24mm，航高一般500米左右，做1：1000地形图很不错。
![6.1.1.jpg](https://i.loli.net/2021/01/23/Iv8XkePjlmQMNBL.jpg)
&emsp;&emsp;相机设置为快门优先，快门速度1/1250，ISO一般设置640以下，一般400
&emsp;&emsp;存储格式精细，相机自动关机的时间设置为最长（30分钟）
![6.1.2.jpg](https://i.loli.net/2021/01/23/SxWRiD4OwhaB1kd.jpg)
![6.1.3.jpg](https://i.loli.net/2021/01/23/CVf5kzYK3mQIeLq.jpg)
#### 6.2 快门线的使用与配置
&emsp;&emsp; <font color='red'> 注意：快门线虽然和USB的接口形状类似，但是里面的引脚数量完全不一样，一定要注意区别。  </font>  
&emsp;&emsp;我使用弯头快门线，极大减小相机舱需要的体积，集成高速光耦，实现飞控端与相机端的信号隔离，保护相机；  
&emsp;&emsp;快门线最大外形尺寸：143*148*164mm，支持飞控信号电平：3.3v-5v，棕色代表地线、橙色代表信号线；  
![6.2.1.jpg](https://i.loli.net/2021/01/23/QObFonK2auBhS4i.jpg)
&emsp;&emsp;<font color='red'> 注意：这个快门线可以给RX2供电5V，但是不支持给A7R供电，因为A7R需要的最低电池电压为7.2V，A7R需要专门的假电池供电。 </font>
![6.2.2.jpg](https://i.loli.net/2021/01/23/WdSRmbEoZBfeutq.jpg)

快门触发配置流程：

1.硬件连接，我使用的AUX1（SERVO9）作为相机的触发口
![6.2.3.jpg](https://i.loli.net/2021/01/23/3c6sQlMtP9J17Di.jpg)
2.在地面站的全部参数列表里面配置CAM_TRIGG_TYPE=1，RELAY_PIN=50；
![6.2.4 .jpg](https://i.loli.net/2021/01/23/L5FE9cj3MaItABd.jpg)
3.在地面站全部参数列表里面，配置SERVO9_FUNCTION=10
![6.2.5.jpg](https://i.loli.net/2021/01/23/TZmax8AP5yNIDs4.jpg)
4.在飞行数据界面里面，点击“Trigger camera Now ”“执行动作”就可以听到清脆的快门声了。
![6.2.6.jpg](https://i.loli.net/2021/01/23/NHmlwIb1ZjV3AWO.jpg)

#### 6.3 相机外接电池的使用
&emsp;&emsp;一般情况下，一个飞行架次， 相机的电池是够的，外接电池主要是为长航时飞行准备的。  
&emsp;&emsp;假电池和实际相机电池的大小是一样的，电源端口接3-6S电池就可以正常工作了。
![6.3.1.jpg](https://i.loli.net/2021/01/23/SUCRKV7ykzs6YJI.jpg)
<font color='red'> 注意：供电线是红极，棕负极 </font>
![6.3.2.jpg](https://i.loli.net/2021/01/23/zAWhqmVkuiQCS3U.jpg)
可以看到显示电量92%，可以正常工作了
![6.3.3.jpg](https://i.loli.net/2021/01/23/SDBMuergcH8waod.jpg)
#### 6.4 为什么相机需要检校
&emsp;&emsp;相机检校的目的是为了检校出像主点的偏移量、畸变参数等重要信息，是摄影测量应用的基础工作，相机检校的精度会直接影响到后期摄影测量成果的精度。  
&emsp;&emsp;相机检校需要检校相机的内方位元素，具体包括（f，X0，y0，k1，k2，p1，p2）。（f，X0，y0，k1，k2，p1，p2）只是众多表示相机成像系统误差模型中的一种，这只是摄影测量领域用的最多的一种误差模型，也叫摄影测量标准模型（photogrammetry standard model）  
&emsp;&emsp;我使用sony 35mm的定焦镜头，定焦镜头在对焦过程中的主距也会发生变化。  
&emsp;&emsp;<font color='red'> 注意：定焦镜头只是不能大范围调焦，可以对着无穷远的地方，旋转对焦环，让照片变得清晰。 </font>  
&emsp;&emsp;我采用的类似棋盘格的相机自检校方法，采用易检校软件，检校报告如下：
![6.4.1.jpg](https://i.loli.net/2021/01/23/TqiYeo5ZJnOmCr9.jpg)
![6.4.2.jpg](https://i.loli.net/2021/01/23/pGxTjuyfA8Sk5mD.jpg)
#### 6.5 相机减震座的使用
&emsp;&emsp;使用EVA材质的相机减振座，一方面方便固定好相机位置，另一方面滤掉一些电机产生的振动，保证高质量的拍摄。
![6.5.1.jpg](https://i.loli.net/2021/01/23/csPaAp5RKlQrBTg.jpg)
![6.5.2.jpg](https://i.loli.net/2021/01/23/drkNm7ByLQxnsPv.jpg)
![6.5.3.jpg](https://i.loli.net/2021/01/23/4iJWzrvY8tGFTM3.jpg)
![6.5.4.jpg](https://i.loli.net/2021/01/23/m1otIzpQUexnhDd.jpg)

### 7 机械电子设备安装

#### 7.1 飞控安装
&emsp;&emsp;飞控安装前，先拆开飞控检查，气压计是否有海绵覆盖，（气压计测量精度容易受光照影响，浅色外壳的飞控要避免在阳光下暴晒）  
&emsp;&emsp;飞控箭头的方向，指向飞控的前方。  
&emsp;&emsp;飞控用3M胶固定，同时3M胶也有一定的减震作用。  
![image.png](https://i.loli.net/2021/01/23/gAfZ1YBaWMhOXk2.png)
&emsp;&emsp;因为布线或者空间有限，需要改变飞控的安装方向，可以调整 AHRS_ORIENTATION参数为合适的值。    
&emsp;&emsp;横滚值向右为正，俯仰值向上为正，方向值顺时针为正。  
&emsp;&emsp;改变方向后需要重新校准水平。我这里就使用标准的安装方法。    
![7.1.1.jpg](https://i.loli.net/2021/01/23/bt1ZmocjpvsNKiC.jpg)
&emsp;&emsp;飞控的位置一般安装离飞机的重心有一定距离，在参数列表里面可以进行偏移补偿  

&emsp;&emsp;因为飞控有2套IMU，都需要进行设置，偏移位置可以设置为相同的值，如果有3套IMU也是相同的设置方法。  
INS_POS1_X   
INS_POS1_Y  
INS_POS1_Z  
INS_POS2_X   
INS_POS2_Y  
INS_POS2_Z  
&emsp;&emsp;飞控固定好以后就蜂鸣器，尽量离飞控远一点，至少5CM。
![7.1.3.jpg](https://i.loli.net/2021/01/23/1lsMYg7n53cHPth.jpg)
&emsp;&emsp;解锁开关也需要固定好（直接穿过飞控舱的泡沫洞即可），同一个设备的线材尽可能绞在一起，一方面简洁美观，另一方面有一定的抗干扰作用。  
&emsp;&emsp;空速计使用I2C的连接方式，线材很容易被干扰，误码率偏高，一方面尽可能减小线材的长度，另一方面空速计的四根线绞在一起。  
&emsp;&emsp;通道信号线的接法：  
&emsp;&emsp;1通道并联两根左右副翼舵机线  
&emsp;&emsp;2通道接左尾翼  
&emsp;&emsp;3通道并联两根接左右机翼的电调控制信号线  
&emsp;&emsp;4通道接右尾翼  
&emsp;&emsp;GPS接飞控的GPS口，GPS安装的时候注意尽可能放在高一点的地方，要求没有任何遮挡地面对天空，尽可能远离动力电源线。  
&emsp;&emsp;GPS接上以后飞控可以自动匹配，自己需要配置GPS安装的偏移量，我这里只接了一个GPS。  
&emsp;&emsp;向前为正X  GPS_POS1_X  
&emsp;&emsp;向右为正Y	GPS_POS1_X  
&emsp;&emsp;向下为正Z	GPS_POS1_X  
![7.1.5.jpg](https://i.loli.net/2021/01/23/HwgEGCuYzfjlKdW.jpg)
#### 7.2 动力设备安装
动力设备接线是最容易错的，一定要非常注意，拿到电流连接器以后注意后面有标号。  
A1—电源负极  
A2—电源正极  
1—电调信号地  
2—电调信号线  
3—舵机信号地  
4—舵机正极  
5—舵机信号线  

大电流连接器的焊接，温度不要持续过高，不然接头塑料容易烧软、变形。


<font color='red'> 注意：机翼部分用的大电流连接器默认为内针（按照XT90插头的惯例） </font>

机身的舵机供电部分是特别需要注意的部分，现在所有的舵机都是从BEC取电，BEC和所有的舵机线在飞控的接线处，正极是并联在一起的，负极是并联在一起的。










