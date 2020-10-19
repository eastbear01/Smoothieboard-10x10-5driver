# Smoothieboard-10x10-5driver
Modified according to [Smoothieboard v1.1 5driver](https://www.reprap.org/wiki/Smoothieboard), a more compact and cost-effective design.

## Pinout

官方抽不出人手绘制fritzing风格的pinout，我就当一次美工哈，根据[Smoothieboard v1.1的pinout](http://smoothieware.org/pinout)乾坤大挪移，可以与原版对比着看

![](https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/Smoothie-10x10-pinout-map-mini.png)

[Full size version](https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/Smoothie-10x10-pinout-map-full-size.png)

## Pin capabilities

![](https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/Smoothie-10x10-pin-capabilities-mini.png)

[Full size version](![](https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/Smoothie-10x10-pin-capabilities-full-size.png))

## 详细指南

见根目录的：冰沙主板制作笔记.pdf（约30MB）

## 为什么要将冰沙主板缩小为10x10？

由于10x10的四层板打样的价格越来越低，而大于10x10的四层板价格仍居高不下，相信不少尝试制作原版冰沙板的大侠一开始就被昂贵的打样费用劝退，因此设计出10x10的冰沙板很有意义，但冰沙主板作为开源了4年以上的开源硬件，其他大佬也设计过不少衍生版本，这些就包括：C3D Remix Board、SKR V-1.3、Cohesion3D Mini、Tiny Smoothie等，似乎我们的选择有很多，然而就如同官方所说的一样，尽管替代形状的数量越来越多，但是**原始设计**（[Smoohieboard v1.1）能为中小型CNC机器（包括但不限于3D打印机，激光切割机和CNC铣床）供电和控制所需的所有电子零件：步进电机驱动器（5通道），加热器/冷却器驱动器（6通道Mosfet PWM），温度传感器（4通道），限位开关，SPI，I2C和用于硬件扩展的其他I / O，其中包括USB，UART，以太网和SD卡。替代设计也应包括这些元素或它们的类似物，或说明如何轻松添加它们。（实际上衍生的设计或多或少都打了折扣）

目前衍生的设计与冰沙板的**相似性**并不太好，对初次接触衍生的主板、阅读原版的文档来学习如何使用冰沙板的朋友们不太友好，因为你需要知道衍生版相比原版的区别（引脚图变动、电子元件变动、布局变动等），因此本id(oldgerman)不另起炉灶，索性直接修改原版的Eagle工程，保留了官方原版（Smoohieboard v1.1）所有的元件和引出的连接器，并适度优化，设计出了Smoothieboard v1.3（10x10），做到原版极其相似的同时，缩小的代价仅仅是大功率MOS的载流需要从原来的12.5A降低至11A(20温升)。

## 命名问题

因为商标问题，Smoothie文档明提到衍生设计不能以”Smoothie XXX“命名，因此我Oct 17号给Smoothie项目的创始人Author Wolf发送邮件并附带了源Eagle工程及下方的指南，希望官方能对此设计提出修改建议，或将该设计纳入官方的设计，或合并到Smoothieware项目中，或拒绝纳入。由于迟迟没回邮件，因此提前将本工程发布到本id的仓库中，以官方的Smoothie命名的方式，命名为Smoothieboard-10x10开源，若后续有变动，文档会添加相关说明。

## Pictures

<table>
    <td><image src = https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/三周目成品(1).jpg></td>
    <td><image src = https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/三周目成品(2).jpg></td>
    <td><image src = https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/三周目测试.png></td>
</table>
## 开源硬件(OSHW)

冰沙主板10x10 是开源硬件

<table><td><img width = 100px height = 100px src = https://github.com/oldgerman/Smoothieboard-10x10-5driver/blob/master/image/Oshw-logo.png></td></table>

可以在[OSHWA.org](http://www.oshwa.org/definition/)上找到OSHW定义的v1.0 

## Acknowledgments

+ The Smoothieboard creators and the [Smoothieware](http://smoothieware.org/) team
+ [捷配小可爱小路路](https://space.bilibili.com/479375532?from=search&seid=14974028502933777239)

