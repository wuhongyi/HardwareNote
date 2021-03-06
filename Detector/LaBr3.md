<!-- LaBr3.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 二 6月  6 14:23:24 2017 (+0800)
;; Last-Updated: 日 9月 24 18:12:53 2017 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 28
;; URL: http://wuhongyi.cn -->

# LaBr3

关于PSD [Enhanced α-γ Discrimination in Co-doped LaBr 3 :Ce](http://wuhongyi.cn/HardwareNote/pdf/Detector/enhanced_a-g_discrimination_in_co-doped_labr3_ce.pdf)

文献：

Kan Yang / Peter R. Menge  FFT法
- 2012
	- [Performance Improvement of Large Sr2+ and Ba2+ co-doped LaBr3:Ce3+ Scintillation Crystals](http://wuhongyi.cn/HardwareNote/pdf/article/06551113.pdf)
- 2013
	- [Scintillation Properties and Temperature Responses of Cs2LiLaBr6:Ce3+](http://wuhongyi.cn/HardwareNote/pdf/article/06829676.pdf)
- 2014
- [Enhanced alpha-gamma Discrimination in Co-doped LaBr3 :Ce](http://wuhongyi.cn/HardwareNote/pdf/article/07431223.pdf)
- 2015
	- [Design and Performance of a Compact Cs2LiLaBr6(Ce) Neutron / Gamma Detector Using Silicon Photomultipliers](http://wuhongyi.cn/HardwareNote/pdf/article/07581858.pdf)  
- 2016
	- [Enhanced alpha-gamma Discrimination in Co-doped LaBr3 :Ce](http://wuhongyi.cn/HardwareNote/pdf/article/07407503.pdf)  



*其它方法*

- 2005
	- [Pulse-shape discrimination of La halide scintillators](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900205000070-main.pdf)
- 2016
	- [Quantitative analysis and efficiency study of PSD methods for a LaBr 3 : Ce detector](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900215016253-main.pdf)  
- 2017
	- [Shape of intrinsic alpha pulse height spectra in lanthanide halide scintillators](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900217302255-main.pdf)

*能量分辨*

- 2012
	- [High rate read-out of LaBr(Ce) scintillator with a fast digitizer](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900212002896-main.pdf)  





----



XIA算法合适参数 SL：1.0 SG：0.24 RANGE：1 TAU：0.06（500MHz）

----


3英寸探头，型号KLB7676。高压+600V，漏流0.27mA。负信号，噪声在正负0.5mV，上升时间20ns，下降时间40+ns。


----

## DT5730测试

源
- Cs137 0.662MeV
- Co60 1.173/1.332 MeV

3英寸高压加到+800V，噪声在正负 1mV 多（50欧姆观察）


获取参数：波形记录1024个点，PreTrigger300个点。阈值8700，DC Offset-40

通过QDC积分得到能量，trigger点前20个点，trigger点后100个点。0.662MeV分辨在3.5%，1.173MeV分辨在2.8%，1.332分辨在2.6%。

看到奇怪的现象，峰的右边有拖尾。


20170922加+1300V，0.662MeV输出信号幅值160mV。QDC积分pretigger点20。posttrigger点60。分辨3.3%。



----

1英寸+PMT，噪声在正负 1 mV 以内（50欧），上升时间6ns内，下降时间40ns左右。

- 高压-1100V，0.662MeV分辨在3.6%（500mV信号）
- 高压-1000V，0.662MeV分辨在3.8%（200mV信号）

峰型很对称

-----

1英寸+XP2020PMT




<!-- LaBr3.md ends here -->
