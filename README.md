# Design-of-Infrared-Thermometer

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f86407db2a1345bbaf98711706c49748.png)

## 1、红外测温仪

经过新冠疫情的洗礼，大家对红外测温枪应该不陌生。在公共场所、企业单位乃至家庭门口，它都成了守护健康的第一道防线。然而，关于红外测温枪有个细节常被误解——它那闪烁的红点，大部分人会认为就是用这个红色的点测量人体温度。其实这个红点并非直接用于测量体温，而是起到了瞄准的辅助作用。
今天就来详细了解一下红外测温仪：**测温原理、红外传感器、光电效应、PIN型光电二极管**。

## 2、红外测温原理

在自然界中，一切温度高于绝对零度（-273℃）的物体，由于它内部热运动的存在，就会不停地向周围空间辐射电磁波，其中就包含了波段位于0.75~100μm红外电磁波。物体的表面温度与其辐射的红外电磁波能量是成正比的。红外测温仪基于这一原理，通过测量目标物体发出的红外辐射能量来计算物体的实际温度。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/33fedc8fa59e4b6595ad7103778b8c69.png)

目标物体发出红外辐射，红外测温仪的光学系统汇聚其视场内的目标红外辐射能量，使红外能量聚焦在光电探测器上，光电探测器将红外辐射能量转变为相应的电信号，该信号再经过放大器和信号处理电路的处理，并按使用特定的算法最终转变为被测目标的温度值。

#### 红外测温的发展

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4a73653933b845bc85a45d02777c63d1.png)

红外测温技术的发展历程可以追溯到1800年，威廉·赫谢尔首次发现了红外线。19世纪末和20世纪初，红外测温技术才开始逐渐应用于实际测量中。

> 1828年，M’Sweeny制造出了第一台辐射温度计，这是红外测温技术的初步尝试。
> 19世纪末，消隐光学高温计的出现标志着红外测温技术开始走向成熟。这种高温计能够测量高温物体的温度，但测量范围有限。
> 1901年，Fery获得了全辐射测温仪的专利，为红外测温技术的发展奠定了基础。
> 20世纪30年代，商用全辐射测温仪问世，使得红外测温技术开始广泛应用于工业领域。


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/bf3a7193e8f445f691a612a954d88777.png)


近几十年来，随着科技的进步和人们对温度测量需求的提高，红外测温技术得到了迅猛发展。红外辐射温度计、红外热像仪、比色温度计、辐射扫描温度计等高科技产品层出不穷。如今，红外测温技术已经广泛应用于电气安装、检测、运行等领域，它能在不接触电气设备的情况下，快速、准确、直观地得出运行中的设备表面温度数据，为人们的生产生活带来了极大的便利。

## 3、红外传感器

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c3c9006ef6b34467821876aaab87d59b.png)

**红外测温仪的核心部件为红外传感器**，红外传感器是利用红外线的物理性质来进行测量的传感器，它以红外线为介质来完成测量功能。以下是对红外传感器特点：
**非接触式检测**：红外传感器测量时不与被测物体直接接触，从而避免了因接触而产生的物理破坏，同时保证了检测的准确性。
**检测精度高**：红外传感器能够精准地检测目标物体的特征变化，具有很高的测量精度。
**响应速度快**：红外传感器的响应时间通常很短，适用于实时性要求严格的应用场景。

#### 红外传感器的分类

红外传感器主要可以分为**热传感器**和**光子传感**器两大类。

**热传感器**
热传感器利用入射红外辐射引起传感器的温度变化，进而使有关物理参数发生相应的变化，通过测量这些物理参数的变化来确定红外传感器所吸收的红外辐射强度。热传感器波段宽、响应时间较长，灵敏度较低。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4ef8eb7cdb15471aaf37f52b71bf6acc.png)

**典型应用**
热电堆传感器：基于塞贝克效应（Seebeck effect）机理。当热电堆的两边出现温差时，会产生电流，可以测量小的温差或平均温度。采用硅基微加工工艺，在硅片支撑层上排布若干对具有不同塞贝克系数材料的热电偶，把这些热电偶串联起来，就构成热电堆芯片。通过测量电压的变化，可以得知入射红外辐射的强度。

热释电传感器：一种具有极化现象的热晶体或“铁电体”。当红外辐射照射到极化铁电片表面时，使片材温度升高，极化强度降低，表面电荷减少，相当于释放了一部分电荷。输出信号的大小取决于板材温度变化的速度，从而反映入射红外辐射的强度。

#### 光子传感器

光子传感器利用某些半导体材料在入射光的照射下产生光子效应，从而改变材料的电学特性。通过测量电学特性变化来确定红外传感器所吸收的红外辐射强度。**光子传感器灵敏度高、响应速度快、探测波段较窄**。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e4101dfba5824f4e95e4c2ef0e9cb5fa.png)

**典型应用**
外光电传感器：当光照射在某些材料的表面时，如果入射光的光子能量足够大，材料的电子就可以从表面逸出。这种现象称为外部光电效应或光电子发射效应。

光电导传感器：当红外辐射照射在某些半导体材料表面上时，半导体材料中有些电子和空穴可以从原来不导电的束缚状态变为能导电的自由状态，使半导体的导电率增加。

光生伏特传感器：当红外辐射照射在某些半导体材料的PN结上时，在结内电场的作用下，自由电子移向N区，如果PN结开路，则在PN结两端便产生一个光生电动势。
**本文主要针对光电导类型传感器进行讲解。**

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e40df58933c641cc922a90c1309904d5.png)


## 4、光电效应

红外光电传感器工作的物理原理是：**光电效应**。光电效应是什么？

![请添加图片描述](https://i-blog.csdnimg.cn/direct/c441db7885b6471fbf85a85eaec598e3.gif)

光照射到物质上，引起物质的电性质发生变化。这类光变致电的现象被统称为光电效应（Photoelectric effect）。光电效应可分为:**光电子发射、光电导效应和光生伏特效应**。光电子发射现象发生在物体表面，称为**外光电效应**。光电导效应和光生伏特效应发生在物体内部，称为**内光电效应**。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d2ae72fd0d2c42ff8b5a8589075f63a0.png)

**光电子发射**：当光照射到金属或某些非金属表面时，若光的频率超过一定阈值，物质表面的电子会吸收光子能量后逸出表面，形成光电流，典型应用为光电倍增管。

**光电导效应**：光照射到半导体表面时，半导体内部的电子获得能量从价带跃迁到导带，从而增加半导体的电导率。典型应用为光电二极管。

**光生伏特效应**：光照使不均匀半导体或半导体与金属结合的不同部位之间产生电位差的现象。典型应用为光伏太阳能板。

#### 红外光电传感器工作原理

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/02890d0947034b94943bc9f25bd2cc23.png)


**红外光电探测器主要利用的是内光电效应**。
光照射在半导体材料上,光子将能量转移到半导体材料的原子中,将空穴和电子（载流子）激发到导态。**在半导体耗尽区内释放出的载流子组成了光电流的主要部分**,主要是因为耗尽区的内建电场对载流子的加速作用，为载流子增加了传导能量，减少了复合概率。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/3f61335a14f94dfa8a7f9a60ba4251cd.png)

此外在耗尽区以外释放出来的载流子在半导体材料里面**扩散**,这些载流子有些被复合，有些到达耗尽区，**到达耗尽区的载流子**在电场加速作用下被传送到二极管的两端（电子向N区移动，空穴向P区移动。），成为光电流的另外一部分。
PN结外加反向偏置电压,可以扩大耗尽区,使更多的半导体材料成为载流子加速区。通常情况下,只有在耗尽区一个扩散长度内生成的载流子才会成为光电流。

扩散长度：**它通常定义为载流子从生成点开始，通过扩散作用能够到达某个特定区域（如耗尽区边缘）的最大距离**。扩散长度是一个描述载流子在半导体中扩散能力的物理量。这个距离受到多种因素的影响，包括半导体的材料特性、温度、掺杂浓度等。

## 5、光电二极管分类

光电二极管（Photodiodes）是二极管的一种，它是很多光学测量中常用的传感器类型，可用于吸收和发射光谱、色彩测量、温度测量、气体探测等应用，以实现精密光学测量。

根据不同的分类标准，光电二极管**按结构可以分**为两类：**PN型和PIN型。**
**PN型光电二极管**是最常见的二极管类型之一，由P型半导体和N型半导体的结合而成。具有结电容小、渡越时间短、灵敏度高等优点，但暗电流小，响应速度一般较低。通常用于照度计、彩色传感器、分光光度计、照相机曝光计等。
**PIN型光电二极管**是在P区与N区之间生成I型层（本征层），吸收光辐射面产生光电流的一种光检测器。具有结电容小、渡越时间短、灵敏度高、响应速度快等优点，但暗电流大，结容量低。通常用于高速光的检测、光通信、光纤、温度测量等。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c4f862f769484a039317500f4b972098.png)

光电二极管按**照制造材料的不同**，主要可以分为以下几类：
**硅（Si）光电二极管**
硅是半导体材料中应用最广泛的一种，具有优良的导电性能和稳定性。硅基光电二极管通常具有较高的灵敏度和可靠性，适用于多种应用环境。
常用于商业化和低成本产品中，如光通信、图像传感器、光电探测等领域。
**锗（Ge）光电二极管**
锗也是一种常见的半导体材料，与硅相比，锗在某些方面具有更高的灵敏度，尤其是在红外光谱范围内。然而，锗的成本相对较高，且易受温度影响，稳定性稍逊于硅。
通常用于需要高灵敏度的特定应用，如红外探测、光谱分析等。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/88cd4defc5cf4d97bbe82e586df9c1df.png)


**砷化镓（GaAs）及铟镓砷（InGaAs）光电二极管**
砷化镓和磷化铟镓是具有优良光电性能的化合物半导体材料。它们具有较高的电子迁移率和较低的光吸收系数，使得这些材料在高速、高灵敏度的光电探测中具有显著优势。
常用于高速光通信、光纤通信、激光雷达（LiDAR）等领域，以及需要宽光谱响应和高量子效率的应用。
**其他材料光电二极管**
量子点光电二极管,利用量子点的独特性质，能够在特定波长范围内实现高效率的光转换。这种二极管通常具有可调谐的光谱响应和较高的灵敏度。
二维材料光电二极管：如石墨烯、过渡金属二硫化物（TMDs）等二维材料，具有优异的光电性能和机械柔韧性。这些材料在光电探测、柔性电子等领域具有广阔的应用前景。
有机光电二极管（OPD）利用有机材料的光吸收和载流子传输特性，具备柔性和可塑性。有机光电二极管在可穿戴设备、有机太阳能电池等领域具有潜在的应用价值。
**本文重点介绍PIN型光电二极管。**

![。](https://i-blog.csdnimg.cn/direct/a38d484038c0436790dd6f21e49c7575.png)



## 6、PIN型光电二极管

**PIN二极管的结构由P型半导体、Intrinsic半导体和N型半导体三层组成**。Intrinsic半导体层是一层轻掺杂的半导体（自由载流子数量少可忽略）。这种三层结构是PIN二极管区别于普通PN结二极管的主要特征。
**本征层（I层）**：本征层是PIN二极管的核心部分，其宽度和掺杂浓度对二极管的性能有重要影响。较宽的本征层使得载流子在其中的渡越时间较长，从而影响了二极管的开关速度。同时，本征层的低掺杂浓度使得在反向偏置时，电子和空穴在I层中移动需要克服较大的空间电荷区，导致漏电流较低。
**重掺杂的P型和N型半导体**：P型和N型半导体层通常是高掺杂的，以提供足够的载流子浓度。在正向偏置时，这些载流子会进入本征层并复合，导致二极管的阻抗降低。![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/eba8c08f592c479b874d68803e099234.png)
一个平衡条件下的PIN二极管如下图所示，PIN二极管是**三层两结**结构，存在P,I,N三个层，存在两个结即 J1和J2结，中间的区域杂浓度很低，在工作时表现为本征特性。此时在J1结和J2结上会产生自建电场，形成空间电荷区。由于P层和N层的载流子浓度比I层高，因此它们的结左右是非对称，P层N层结厚度较薄。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e9853d53fecb445cb1487ad5c79b4811.png)

**光生电流的产生**
在光电二极管增加了一个本征层，扩大了耗尽区,因此提高了响应的光谱范围。**光子在半导体中释放载流子的深度范围与光子波长成比例**，而且只有那些在耗尽区内部或附近释放出的载流子才能转化为二极管电流。
当红外光照射到PIN二极管的P型或N型半导体区域时，光子会被半导体材料吸收。吸收光子后，半导体材料中的电子会获得足够的能量从价带跃迁到导带，产生电子-空穴对。这些电子-空穴对在内建电场的作用下发生分离：电子向N区移动，空穴向P区移动。
在I层中，由于载流子浓度很低，电子和空穴的移动相对缓慢。然而，当红外光照射到I层时，也会产生电子-空穴对。这些电子-空穴对在内建电场的作用下也会发生分离，并在I层中形成光生电流。由于I层的宽度较大，电子和空穴在I层中的移动需要克服较大的空间电荷区，因此光生电流在I层中的流动相对较弱。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f3c4a8b39688494a897faca2563e1b5e.png)


## 7、红外光电二极管

为了加强对红外光电二极管的了解，通过一款光电二极管来学习光电二极管的参数。根据G10899的参考手册可以得到以下关键信息：

> 1、它是一个PIN型光电二极管
> 2、它使用的是铟镓砷（InGaAs）材料 
> 3、它适用于0.5~1.7um 4、它适用于做红外测温


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/09c7c0a0c01d4510b2ddf2555f577c76.png)

根据手册可以发现以下重要参数：

> 1、中心波长，是指PIN光电二极管对光信号响应最灵敏的波长。
> 2、光敏性，是指PIN光电二极管对光信号的敏感程度，即光信号转化为电信号的能力。
> 3、暗电流，是指在无光照条件下PIN光电二极管内部产生的微弱电流，一般在几个纳安（nA）。
> 4、结电容，电容是指PIN光电二极管内部P-N结形成的电容。PIN光电二极管的结电容较小，一般为几十皮法（pF），较小的结电容使得PIN光电二极管的响应时间较短。


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/d4bc1f6888ec4cccbfa56d37d2494953.png)


## 8、测量电路设计

接下来介绍一下光电二极管的测量电路，该电路主要分为4个部分：**光电转换电路、信号滤波电路、二级放大电路、模数转换电路**。


![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/703e3aa0a8134bdabc7d3695f66796e7.png)

**光电转换电路有以下3个方案**：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/e0be41af9ccf4597b2791a116e46e338.png)


**滤波电路有以下2个方案**：

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4a2ffeafa6b74e458bcd49040f0c032c.png)


二级放大电路和模数转换电路设计比较简单，在这里就不一一介绍了。

## 9、总结

本文内容分为以下几点：
1、红外测温仪应用以及其工作原理
2、红外传感器的分类以及光电效应
3、光电二极管以及PIN型光电二极管
4、测量电路设计

**创作不易希望朋友们点赞，转发，评论，关注!
您的点赞，转发，评论，关注将是我持续更新的动力!
CSDN：https://blog.csdn.net/li_man_man_man
今日头条：https://www.toutiao.com/article/7149576260891443724**
