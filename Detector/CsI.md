<!-- CsI.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 三 5月 24 21:09:32 2017 (+0800)
;; Last-Updated: 三 3月  6 13:52:36 2019 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 15
;; URL: http://wuhongyi.cn -->

# CsI 探测器

5.4 MeV alpha 注入深度大约为 27.7 um

- [Charged-particle detection efficiencies of close-packed CsI arrays](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900216313122-main.pdf)




## 晶体的包装

CsI晶体需要在入射面和光接收面打磨光滑，**明显可以看出是透明的效果**（加工的时候要求，还需要要求尽可能加工的平整）。

包装可能要用到的材料：

- 2um mylar膜
- 10um mylar膜
- 生料带
- 硅脂
- T开头的一种纸（一种有点厚的纸）
- 土豪金胶带



耦合PD/APD或者光电倍增管。

PD有金丝的为正信号，没有金丝得为地线。与硅类似，可以选择正面加高压也可以选择背面加高压。给金丝加负高压，输出信号为负信号，给地线加正高压，输出信号为正信号。

PD漏流应该在几个nA才合理。


耦合前应该用酒精先把CsI擦洗干净。在耦合面中心点上一点硅脂，然后PD水平放上去，轻轻挤压，让硅脂从中间一点扩散到整个面，这样的方法才能保证里面尽可能的不留下气泡（里面如果有气泡，抽真空之后气泡将会变得很大）。

耦合光电倍增管也是类似的。

关于侧面的包装，原则是包裹的越紧越好，根据实验探测器的摆放空间问题，选择不同的包装方式。

如果要测重带电粒子，前面入射窗面需要包 2um mylar膜（越薄mylar膜所带来的能损越小，mylar膜越厚，其自身厚度不均匀性所带来的能损差异较大），mylar膜的包装需要尽可能的拉平。如果仅仅测gamma射线，则入射窗面的处理可以与侧面的一样。

侧面的处理，如果空间足够的话，用生料带往侧面捆个五六圈（或者更过的）的就可以了。如果需要包的薄一些，可以先用生料带紧密包上一两圈，主要是生料带可以包的很紧，然后包一圈10um mylar膜，外面再包一圈Taylor纸。

----

## 关于PSD

*Short/Long*

- 2016
	- [Pulse shape discrimination properties of Gd3Ga3Al2O12 :Ce,B single crystal in comparison with CsI:Tl](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900216310130-main.pdf)

*多种方法*

- 2004
	- [Near threshold pulse shape discrimination techniques in scintillating CsI(Tl) crystals](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900204000336-main.pdf)



----

## 测试


耦合PD输出，采用理研的前放，1pF 20M参数

241Am alpha源。前放的噪声大概2mV左右，信号幅度在5mV左右。信噪比在1：1到2：1左右。上升时间在1us左右。

采用传统获取测试需要将其放大足够大，可以采用572A或者N568B主放（主放的信号会看到基线晃动的比较厉害，可能是前放的信号小，放大的倍数太大，基线都给放大了）。对35x35x100mm晶体，测试最好的分辨在**百分之八左右**。晶体越小，分辨应该会好些。如果用光电倍增管，分辨也会较好。


对数字化获取，由于其输出信号幅度小，CAEN插件采用前沿甄别，阈值需要设置的很低才行。XIA插件采用fast filter算法甄别，通过设置好甄别参数（例如FL：1us，FG：0.27us），可以获得较好的触发。还有个问题，如果输入量程较大（0-2V），而精度又较低（例如12bit），那么其高度将只有几个点，不利于能量计算。


----

**20170529**

尺寸35x35x100mm CsI(Tl) 耦合灵敏面积30x30mm的PD（S3584-08），采用理研前放，参数0.5pF、20M

241Am alpha源

降噪做好时，没加高压时候，噪声在正负5mV，加上高压之后，噪声在正负1.5mV，信号幅度10mV，上升时间为1us多。

传统获取采用N568B前放，将信号放大到V785的2000道左右。测量能量分辨最好在7.5%

XIA数字化获取（100M 14bit），能量分辨在 8.5%（通过优化参数应该还有一点提高的空间）。


**20170530**

尺寸15x15x5mm CsI(Tl) 耦合PD（S3204），理研前放，0.5pF、20M

241Am alpha源

加高压之前，噪声在正负5mV，加高压之后，噪声在正负2mV以内。信号幅度15mV

传统获取采用N568B前放，信号放大到ADC3000道左右。







<!-- CsI.md ends here -->
