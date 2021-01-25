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
![7.2.1.png](https://i.loli.net/2021/01/24/8qg4NOMRpmHWoFy.png)
大电流连接器的焊接，温度不要持续过高，不然接头塑料容易烧软、变形。
![7.2.2.png](https://i.loli.net/2021/01/24/gNxTsjQOdkn1vi9.png)
![7.2.3.png](https://i.loli.net/2021/01/24/onHGvaIfr645ZqC.png)

<font color='red'> 注意：机翼部分用的大电流连接器默认为内针（按照XT90插头的惯例） </font>
![7.2.4.jpg](https://i.loli.net/2021/01/24/GlXavLq2IhjbeV1.jpg)  
![7.2.5.jpg](https://i.loli.net/2021/01/24/rFwic7nk2dZmOqp.jpg)

&emsp;&emsp;机身的舵机供电部分是特别需要注意的部分，现在所有的舵机都是从BEC取电，BEC和所有的舵机线在飞控的接线处，正极是并联在一起的，负极是并联在一起的。
![7.2.6.jpg](https://i.loli.net/2021/01/24/3TsCP7BRYg8v91h.jpg)
#### 7.3 遥控系统的安装
&emsp;&emsp;采用天7遥控器，有效距离在几百米的范围，遥控器使用的棒状天线，当天线竖直放置时，围绕天线水平面方向信号最强，而天线头所指方向信号最弱。飞行过程中应根据飞行器的位置适当调整遥控器天线方向使飞行器始终处于天线信号较强的区域范围内，避免飞行器处于天线头所指的方向。
![7.3.1.jpg](https://i.loli.net/2021/01/24/1BXHYc3tOQNDWw5.jpg)

&emsp;&emsp;航测的飞机一般飞得都比较高，为了获得比较好的信号强度，接收机天线，我沿着机身45度安装，信号的距离和高度兼顾。
&emsp;&emsp;天线周围尽量远离其他的电子设置，注意电磁波是很容易穿过泡沫的，我把天线放在外面是为了方便固定角度。
![7.3.2.jpg](https://i.loli.net/2021/01/24/6M2AwGBDXrqyl98.jpg)

#### 7.4 数传系统的安装
&emsp;&emsp;数传的天线和遥控器天线的原理是一样的，但是放置的方法有些区别，数传需要获得更远的距离。飞机的巡航高度一般在500米左右，在这种情况下，飞机端的胶棒天线和PCB天线都可以竖立放置。
![7.4.1.jpg](https://i.loli.net/2021/01/24/xtZMTgp7DjlQhLN.jpg)
&emsp;&emsp;注意天线端的两个口，飞控会自动选择信号最好的口连接，建议两个天线都接，也可以只接一个天线。  
&emsp;&emsp;地面端的天线也是竖立，两个口都接大天线，这样获得的信号更好一些。地面端的天线放置尽可能高一些，尽可能避开建筑物的遮挡。  
&emsp;&emsp;这样的配置，飞机在离家近的地方信号差一点，但是可以获得更远的距离。  

#### 7.5 降落伞安装
##### 机身伞绳安装：
![7.5.1.jpg](https://i.loli.net/2021/01/24/yK6A2QilknuFs4a.jpg)
&emsp;&emsp;适当调节每根伞绳长度保证伞绳的中心在飞机重心稍微靠前的位置，这样飞机抛伞后也能保持机身水平，保证降落稳定。
![7.5.2.jpg](https://i.loli.net/2021/01/24/JBcODoGebPFjVvX.jpg)
&emsp;&emsp;确定好机身每根伞线的长度后可以固定伞结，用带垫的螺丝拧紧。（银燕ES3154舵机配件包里面的代垫螺丝即可）。
![7.5.3.jpg](https://i.loli.net/2021/01/24/nIBP3qSY1Jhg6vz.jpg)
&emsp;&emsp;拧好以后检查一下松紧度，确保伞绳部分在凹槽中
![7.5.4.jpg](https://i.loli.net/2021/01/24/LZYW2IwENy4SVQr.jpg)
&emsp;&emsp;规整好伞绳后用束线帽固定住，保持整齐
![7.5.5.jpg](https://i.loli.net/2021/01/24/arQeniCkcTqBNfu.jpg)
&emsp;&emsp;尾部同样用束线帽固定稳当，整个机身伞绳就这样固定好了。
<font color='red'>  
手动开伞  
优势：开伞灵活，可以多次开伞  
劣势：不能用航线命令开伞  

自动开伞  
优势：可以通过地面站命令开伞  
劣势：只能开伞一次以后，就不能重复开伞了 </font>

##### 手动开伞的设置步骤:
说明：我使用的RC7（也就是遥控器的7通道输入），使用AUX2（也就是飞控的SERVO10）  
连接舵机控制开伞  
![7.5.6.jpg](https://i.loli.net/2021/01/24/6ihT8HRc9ajgAyt.jpg)
这个设置相当于把RC7和SERVO10映射在一起  
##### 自动开伞的设置步骤:
CHUTE_CHAN=7，设置遥控器7通道开伞  
CHUTE_ENABLED=1 使能开伞功能，写入后要重启，可以看到关于伞降的几个新参数  
CHUTE_SERVO_OFF=合适的值  调整舵机关闭位置  
CHUTE_SERVO_ON=合适的值   调整舵机释放位置  
CHUTE_TYPE=10 使用舵机开伞  
SERVO10_FUNCTION=27 舵机SERVO10口，开启降落伞功能  
![7.5.7.jpg](https://i.loli.net/2021/01/24/sDVEHIBjKAc1tO5.jpg)

拨动遥控器开关就可以听到“滴—滴—滴”的开伞，舵机摆动，然后约3秒后复位。  
### 8 飞控初始配置
#### 8.1 加速度校准
点击“校准加速度”按提示放置飞控，可以校准成功，实际上就是六面校准法
![8.1.1.jpg](https://i.loli.net/2021/01/24/VyMgki57OtsNHFe.jpg)
![8.1.2.jpg](https://i.loli.net/2021/01/24/Gtm7jAh4Ne5icby.jpg)
&emsp;&emsp;校准水平，只需要把飞控放平以后，点击校准，飞控灯快速闪烁后完成，表示校准水平成功。校准水平的原因是飞控装在机身里面，或多或少有安装误差，校准水平的目标就是修正偏移误差。
&emsp;&emsp;注意：校准水平只能校准横滚和俯仰轴，若出现校准以后，横滚和俯仰的值没有归零的情况，一般是地面站和飞控固件版本不匹配。
![8.1.3.jpg](https://i.loli.net/2021/01/24/wFxt5cgGXkYfrT3.jpg)

#### 8.2 遥控器校准
&emsp;&emsp;遥控器校准要注意，校准完成后油门位置放在最低，其它通道都要归置中位，不然会有一些奇怪的事情出现.  
&emsp;&emsp;固定翼通道对应功能  
&emsp;&emsp;Channel 1: Roll  
&emsp;&emsp;Channel 2: Pitch  
&emsp;&emsp;Channel 3: Throttle  
&emsp;&emsp;Channel 4: Yaw  
&emsp;&emsp;校准的过程中，摇杆要打到最大值，反复几次。  
![8.2.1.jpg](https://i.loli.net/2021/01/24/RcLDe4YUkniNBOW.jpg)

#### 8.3 遥控器飞行模式配置与失控保持

&emsp;&emsp;我使用的遥控器5通道作为飞控的模式切换开关，在地面站里面需要单独配置（飞控默认8通道作为遥控切换开关）  
FLTMODE_CH=5  遥控器5通道作为飞控的模式切换开关
![8.3.1.jpg](https://i.loli.net/2021/01/24/3QLtDH9fiIzeBR1.jpg)
配置完成后拨动模式开关，检查模式是否正常切换  
![8.3.2.jpg](https://i.loli.net/2021/01/24/cMbOenQukW3TKEi.jpg)
&emsp;&emsp;为了防止飞机飞远以后，出现失控情况，有的接收机的PWM输出就会出现最小值/中位值，在这样情况下，飞控的模式开关就会出现跳变，可能会自动切到手动，引起炸机。  
&emsp;&emsp;现在需要在遥控器的“高级设置”里面的“失控设置”进行配置，我的第5通道，对应为起落架，设置起落架为“失控保持”  
![8.3.3.jpg](https://i.loli.net/2021/01/24/mikjy1MdvBpCTXo.jpg)
![8.3.4.jpg](https://i.loli.net/2021/01/24/HAfS68zeUYoJFDL.jpg)
&emsp;&emsp;设置完成以后，要验证，切换5通道的模式开关到“AUTO”档位，关闭遥控器10 秒以上，观察飞控模式是否发生跳变
![8.3.5.jpg](https://i.loli.net/2021/01/24/vBCa58Tz6fhEdHR.jpg)
#### 8.4 罗盘校准的说明
&emsp;&emsp;我一般固定翼不用罗盘，考虑到有的爱好者喜欢用罗盘，我也把相关配置写下来。  
&emsp;&emsp;罗盘连接I2C口，因为I2C被空速计占用了，需要I2C扩展板（简单地说就是把所有I2C设备并联在一起）    
使用罗盘2作为外置罗盘的配置
![8.4.1.jpg](https://i.loli.net/2021/01/24/W5NRHYPFTSKDarf.jpg)
PIXHAWK目前支持双外置罗盘，现在暂时只用一个外置罗盘，点击“现场校准”
![8.4.2.jpg](https://i.loli.net/2021/01/24/pcFrRlqVJoPs3Mt.jpg)
##### 最快的校准方法：（不要拿着飞机乱转，不然很难通过）  
1.先把飞机指向北方，绕俯仰轴旋转到水平；    
2.再把飞机水平旋转90度，机头指向西方/东方；  
3.再把飞机绕横滚轴旋转至水平；    
#### 8.5 故障保护
&emsp;&emsp;故障保护，一般触发原因：电池没电、遥控器丢信号、地面站数传断开，GPS异常。    
我通常的设置是都不开，原因如下：    
&emsp;&emsp;1.航测作业起飞前就应该检查电池有没电，即使设置电池低电压保护，在大油门情况下，电池压降太大，可能会误触发低电压保护。  
&emsp;&emsp;2.遥控器失控后，通道设置为保持，至少保证“AUTO”情况下不会乱跳模式。   
&emsp;&emsp;3.航测作业中，航线是先写进去了的，一般会预估航程和时间，即使出现障碍物阻挡，导致飞机与地面站失联，飞机也不需要急着返航或者盘旋等待，完全可以继续等航线飞完再回来。    
&emsp;&emsp;4.GPS丢新的情况在空中概率很小，一般买好一点的GPS来用，一般飞行高度都比较高，高空能影响GPS信号的因数很少，只要控制好飞机的转弯角度不要太大，GPS一般没得什么问题，我飞了2000多个起落了高空还没出现丢星的情况。  
![8.5.1.jpg](https://i.loli.net/2021/01/24/BO7vWK4Fo8zTtQA.jpg)
#### 8.6 V尾混控配置
&emsp;&emsp;V尾混控主要是SERVO2_FUNCTION和SERVO4_FUNCTION的功能不一样。  
SERVO1_FUNCTION	4	aileron  
SERVO2_FUNCTION	79	left V-tail  
SERVO3_FUNCTION	70	throttle  
SERVO4_FUNCTION	80	right V-tail  
![8.6.1.jpg](https://i.loli.net/2021/01/24/clhRYfOrZQDwuPt.jpg)
&emsp;&emsp;把飞控切到“手动模式”，检查副翼和尾翼舵面，不平的舵面全部机械调至平衡（也就是舵面的机械中位）。  
&emsp;&emsp;我习惯把机翼和尾翼的混控关掉，因为尾翼和副翼联动，容易引起甩尾现象。  
&emsp;&emsp;KFF_RDDRMIX=0  关掉机翼和尾翼的混控  
![8.6.2.jpg](https://i.loli.net/2021/01/24/eUPAJiygOtl5RDG.jpg)

检查遥控器输入通道与执行动作是否比配

| <font color='red'> <div style="width:280px">遥控器输入通道</div></font> | <font color='red'><div style="width:280px">相应舵面执行的动作</div></font> |  
| :----: | :----: |  
横滚通道往右拨动摇杆 |	左副翼向下运动，右副翼向上运动  
横滚通道往左拨动摇杆 |	左副翼向上运动，右副翼向下运动  
俯仰通道往下拨动摇杆 |	左尾翼向上运动，右尾翼向上运动  
俯仰通道往上拨动摇杆 |	左尾翼向下运动，右尾翼向下运动  
方向通道往左拨动摇杆 |	左尾翼向下运动，右尾翼向上运动  
方向通道往右拨动摇杆 |	左尾翼向上运动，右尾翼向下运动  

&emsp;&emsp;如果检查到舵面方向不对，最好不在遥控器里面改通道正反，因为一个遥控器可能要飞几个飞机，直接在地面站的“遥控器校准”里面。
![8.6.3.jpg](https://i.loli.net/2021/01/24/sZU23Trftk4Ka9O.jpg)
接下来把遥控器的模式开关切换到“FBWA”，检查舵面在“自稳”情况下的反应  

| <font color='red'> <div style="width:280px">飞机倾斜方向</div></font> | <font color='red'><div style="width:280px">舵面动作情况</div></font> |  
| :----: | :----: | 
横滚往右倾斜 | 左副翼向上运动，右副翼向下运动
横滚往左倾斜 | 左副翼向下运动，右副翼向上运动
俯仰向上倾斜 | 左尾翼向下运动，右尾翼向下运动
俯仰向下倾斜 | 左尾翼向上运动，右尾翼向上运动
方向水平向左运动 | 左尾翼向上运动，右尾翼向下运动
方向水平向右运动 | 左尾翼向下运动，右尾翼向上运动

如果运动方向相反，可以在“舵机输出”界面，设置反向
![8.6.4.jpg](https://i.loli.net/2021/01/24/Eg57XVWP1vKd9uI.jpg)
 
<font color='red'> 注意：如果尾翼不管怎么调，方向还是不对的话，可以交换SERVO2_FUNCTION和SERVO4_FUNCTION的设置。 </font>
SERVO4_FUNCTION	79	left V-tail  
SERVO2_FUNCTION	80	right V-tail  
![8.6.5.jpg](https://i.loli.net/2021/01/24/DLutI72fevmdshO.jpg)
按照上述方法一般就可以调好，在调试过程中务必反复检查，谨慎对待。  

#### 8.7 电调校准
&emsp;&emsp;电调校准，主要就是让电调知道遥控器的油门通道的最大值和最小值，电调存储下油门量程的最大值和最小值，通过电机和桨的作用，体现到动力输出上。  
&emsp;&emsp;通过飞控，可以直接同步校准2个电调行程  
&emsp;&emsp;1.移除桨，断开动力电池，只通过USB给飞控上电   
&emsp;&emsp;2.把遥控器切换到手动模式  
&emsp;&emsp;3.BRD_SAFETYENABLE=1  关闭安全开关功能  
![8.7.1.jpg](https://i.loli.net/2021/01/24/1CgMftqISbyBDRZ.jpg)
&emsp;&emsp;4.ARMING_REQUIRE=0  关闭遥控器解锁功能  
![8.7.2.jpg](https://i.loli.net/2021/01/24/BTohevgaGNDIius.jpg)
&emsp;&emsp;5.把油门推到最高，用动力电池，给电调上电  
&emsp;&emsp;6.听到“滴-滴”两声，表示进入到了油门行程校准模式了  
&emsp;&emsp;7.再把油门摇杆推到最低，听到一声“长滴”，表示校准成功  
&emsp;&emsp;8.然后缓慢推动油门，电机就可以旋转了  
&emsp;&emsp;9.校准完成以后，再把安全开关和解锁功能恢复  
  
#### 8.8 配置舵机的正反输出
&emsp;&emsp;舵机在安装的时候需要先使用舵机测试仪把舵机归置大概中位，为什么这么做？    
&emsp;&emsp;主要是保证摇臂两边摆动的行程尽可能一致。   
&emsp;&emsp;舵机归中以后调整舵面，通过调节球头连杆的行程，把副翼和尾翼舵面分别调至中位。	（目测整个舵面看上去是平的）    
&emsp;&emsp;舵机设置以SERVO1为例  
&emsp;&emsp;SERVO1_FUNCTION=4 设置1通道对应功能为副翼  
&emsp;&emsp;SERVO1_MAX=1900 最大PWM值为1900  
&emsp;&emsp;SERVO1_MIN=1100 最小PWM值为1100  
&emsp;&emsp;SERVO1_REVERSED=1 反向输出通道  
&emsp;&emsp;SERVO1_TRIM=1500 舵机中位值为1500  
![8.8.1.jpg](https://i.loli.net/2021/01/24/gnYykKSd5quowUb.jpg)

#### 8.9 关于油门解锁

油门解锁是飞机起飞前的最后一道保证，在按下安全开关以后，所有通道的信号输出都有了。   
解锁之前一定要慎重  
解锁可以配置两个参数  
ARMING_REQUIRE=1	解锁时必须油门在最小值  
ARMING_RUDDER=2  方向向右打到底表示解锁，同理方向向左打到底表示上锁  
![8.9.1.jpg](https://i.loli.net/2021/01/24/C3q5UngoLpXsbR1.jpg)
### 9 第一次飞行调试
#### 9.1 起飞前的必备工作
起飞前的准备工作：  
&emsp;&emsp;1.模拟器能够正常进行起降，已经使用练习机进行了一段时间的实际飞行，有一定的飞行经验，如果这些条件不具备，最好找一位有航模经验的爱好者指导。  
&emsp;&emsp;2.组装好飞机，安装好电池，<font color='red'>注意飞机的重心在机翼下面的凸起处，在重心处双手指尖支撑起飞机，让飞机基本保持水平状态。</font>  
&emsp;&emsp;3.第一个架次觉得飞机重心不合适，要进行调整，否则会出现飞机要么低头、要么仰头很难操控的情况。  
&emsp;&emsp;4.打开遥控器切换到手动模式，然后给飞机接通电池。  
&emsp;&emsp;5.“手动模式”下检查飞机的舵面是否正常，然后切换到“FBWA模式”检查飞机的舵面修正方向是否正常。  
&emsp;&emsp;6.连接地面站，检查空速计是否正常，GPS搜星是否正常。  
&emsp;&emsp;7.用水平珠让飞机放置水平，检查飞控的“横滚”和“俯仰”是否水平，如果没有水平需要加速度计“校准水平”。  
&emsp;&emsp;8.第一次起飞建议用“手动模式”因为手动模式的输出量程比较大，比较容易应对突发情况。  
&emsp;&emsp;9.最后检查飞机的动力，螺旋桨的旋转方向是否正确，电机的最大推力输出是否正常，注意飞行的风向，一般是逆风起飞。  

#### 9.2 自动调参
&emsp;&emsp;自动调参的目的，是让飞机在自动增稳情况下，对舵面的补偿的力量，速度，提前量都很合适。
![9.2.1.jpg](https://i.loli.net/2021/01/24/rwOiCRmeHZjLNxV.jpg)
&emsp;&emsp;先手动起飞，飞行到60-80米切换到“AUTOTUN”模式，现在横滚和俯仰有一点增稳作用，但不是很合适，可能不好飞，不用慌。  
&emsp;&emsp;自动调参校准横滚，快速地拨动横滚摇杆的向左打到底，再向右打到底，连续拨动20下，只要飞机不掉下来，快速拨杆打舵，慢慢地你会发现飞机的横滚增稳有改善。觉得不合适，再重复几次。  
&emsp;&emsp;自动调参校准俯仰，建议先把飞机飞高一些，免得救机的高度不够，快速拨动俯仰摇杆最上到最下，连续20次，可以看到飞机飞波浪线，回中后逐渐会发现飞机的俯仰有改善，如果没得改善继续校准。  
&emsp;&emsp;校准完成后切换到FBWA模式下，感受飞机的操控状态，直到自己满意为止。  
&emsp;&emsp;每个飞机的遥控器行程不一样、舵机中位不一样、连杆到舵面的位置不一样，飞机的起飞重量不一样等因数，导致每个飞机自动调参后的PID都有细微差异，这个是正常的。  
![9.2.2.jpg](https://i.loli.net/2021/01/24/PmB6WIpYy2hfgMC.jpg)

#### 9.3 检测振动对加速度计的影响
&emsp;&emsp;测量加速度计的振动情况主要是：评估电机在飞行过程中振动对飞控加速度的影响是否在正常的范围以内。  
找到之前的飞行日志，然后用地面站打开
![9.3.1.jpg](https://i.loli.net/2021/01/24/MQfZVBIsu8m6XN5.jpg)
打开Vibe X，Vibe Y，Vibe Z这三个参数，观察他们值得范围，只要在60m/s/s以下，都在飞控可以接受的范围以内
![9.3.2.jpg](https://i.loli.net/2021/01/24/EUwn2S97TdkW5uO.jpg)
接下来检查Clip0，Clip1，Clip2这三个参数，只要值在100以下都是正常的
![9.3.3.jpg](https://i.loli.net/2021/01/24/wxQez8HYALpG6Do.jpg)
如果出现值超出正常的范围，就必须要考虑减震的问题了，主要从机械方面入手。
#### 9.4 导航参数调整
导航参数：主要是让飞机和航线比较好的匹配，更好地按照航线飞行。  
调试之前，先配置飞机的巡航速度,全部参数列表里面  
TRIM_ARSPD_CM=1800 巡航速度18m/s  
开启地面站“飞行计划”  
![9.4.1.jpg](https://i.loli.net/2021/01/24/nSRitMAqUab6ef2.jpg)
1.解释第5个命令：  
DO_JUMP 1 -1   前面第一个“1”指的是航点1，第二个“-1”指无限循环，飞机会绕矩形航线一直飞行。  
2.飞机偏离航线太严重，可以调整参数NAVL1_PERIOD=20  20是默认值，飞机偏离航线把值改小，注意不要改得太小，太小飞	机会绕航线S飞行。  
3.飞机转弯掉高增加PTCH2SRV_RLL的值，飞机转弯爬高严重，减小PTCH2SRV_RLL的值。  
4.调好的状态—飞机能压着航线正常飞机，转弯不过度爬高也不掉高。飞机的高度保持在正常的范围内。  

#### 9.5 自动起飞设置

飞机在整个参数调整好以后，再增加自动起飞功能，这样是安全性最高的。
TKOFF_THR_MINACC=4 自动起飞的最小加速度，也就是往前推一下，电机自动打开，这个值的大小可以根据自己的感觉调整。  
TKOFF_THR_DELAY=10 含义是延迟1S以后，电机才开始旋转，这个值也可以根据自己的实际使用情况调整。  
TKOFF_THR_MINSPD =0电机启动前的最小地速，设置为0就可以了  
![9.5.1.jpg](https://i.loli.net/2021/01/24/V7PbaBTpXN8vCyZ.jpg)
配置完整后，重新飞控  
&emsp;&emsp;准备自动起飞之前，一定要检查好舵面补偿方向是否正确，起飞前，一定是逆风起飞，遥控器切换到AUTO模式，前后抖动飞机，飞机的电机开始旋转，等待油门加速到最大值以后，再水平仍出飞机。

### 10 地面站飞行
#### 10.1 相机参数设置
相机参数设置，需要先在地图上画一个多边形，在地图上点击右键“绘制多边形”里面“添加多边形”  
然后点击“自动航点”里面的“Suvey(Grid)”  
![10.1.1.jpg](https://i.loli.net/2021/01/24/ZliGp6djEnyTcbN.jpg)
就可以使用测绘功能了
![10.1.2.jpg](https://i.loli.net/2021/01/24/rtLXx2VzZdpHove.jpg)
&emsp;&emsp;在相机一栏里面外面选择“sony A7R”相机的放置角度选择“Camera top facing forward”  
&emsp;&emsp;表示相机是横着放进相机舱里面的，拍摄出来的照片，每一张都是横着的。  
&emsp;&emsp;选择“Advanced Options”可以进行一些更高级的配置    
![10.1.3.jpg](https://i.loli.net/2021/01/24/k83S7tEfr9osFyC.jpg)
如果有的相机参数，地面站本身没有，可以自己添加一个相机文件进去，然后保存就可以了。
#### 10.2 块状区域航线规划

块状航线是航测最常用的航线方式
![10.2.1.jpg](https://i.loli.net/2021/01/24/6WpuVQt3g24XhZ7.jpg)
配置的参数比较简单，自己可以多调试调试，慢慢就熟悉参数的含义了
![10.2.2.jpg](https://i.loli.net/2021/01/24/LWn6i4crRhvGHmC.jpg)
注意：山区飞行一定要验证一下航线高度合不合适，防止撞山，我们所用的飞行高度一般指相对起飞点的相对高度（不是海拔高度）  
![10.2.3.jpg](https://i.loli.net/2021/01/24/hHt5QfqKWSbsx93.jpg)
&emsp;&emsp;设置过冲距离的目的是：飞机转弯的阶段姿态不好，就不拍摄了，让飞机掉头把姿态调整好。  
&emsp;&emsp;纵横向的重叠率根据实际情况情况进行设置，自己多摸索几次，就比较清楚了。
![10.2.4.jpg](https://i.loli.net/2021/01/24/b9pDL5IiJKgScAH.jpg)
双相机做倾斜摄影，需要飞矩形航线，矩形航线只需要选择“Cross Grid”就可以了。
#### 10.3 带状区域航线规划
“带状区域”的设置比“块状”更加简单，还是需要先画好“多边形”沿着需要测量的管线画，  
然后在地面站里面选择“Corridor”,再设置带状的宽度。   
![10.3.1.jpg](https://i.loli.net/2021/01/24/Eqv8gLQYbBktZRJ.jpg)
可以预估地看到照片覆盖的范围
![10.3.2.jpg](https://i.loli.net/2021/01/24/BYV9E5CZWGKoe76.jpg)
![10.3.3.jpg](https://i.loli.net/2021/01/24/y5hxZdQraFo4lDB.jpg)


生成的航线如图所示
#### 10.4 如何导出POS数据
在飞控设置里面，想让飞机的LOG文件不那么大，可以设置LOG_BITMASK=4096
![10.4.1.jpg](https://i.loli.net/2021/01/24/FXj53HisLGR9d41.jpg)
但是我一般是全是打开，主要是为了分析飞机的异常情况，全部打开以后日志的文件太大，可以通过“飞控POS快速提取工具”方便提取LOG  
先把.BIN文件转为.Log  
![10.4.2.jpg](https://i.loli.net/2021/01/24/5jcyWPw9mpi8FVZ.jpg)
加载.Log文件
![10.4.3.jpg](https://i.loli.net/2021/01/24/GwPBzdaSUmJrMtl.jpg)
可以看到CAM被提取出来了
![10.4.4.jpg](https://i.loli.net/2021/01/24/tn8lerFhpc6DyXV.jpg)
点击存盘，找到提取出来的CAM文件位置就可以了
![10.4.5.jpg](https://i.loli.net/2021/01/24/J8IA3wsvfyicMZB.jpg)

最后，一定要由衷感谢软件的开发者，开发了这么实用的小工具免费给我们用。
![10.4.6.jpg](https://i.loli.net/2021/01/24/i6dlxbDFhLYC2v8.jpg)




