<!-- PMT.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 五 2月 23 19:35:54 2018 (+0800)
;; Last-Updated: 五 2月 23 20:03:18 2018 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 3
;; URL: http://wuhongyi.cn -->

#PMT 


## 常见产品介绍

- ORTEC不带/带前放的PMT
	- [266 Photomultiplier Base](http://wuhongyi.cn/HardwareNote/pdf/Detector/266-mnl.pdf)
	- [276 Photomultiplier Base with Preamplifier](http://wuhongyi.cn/HardwareNote/pdf/Detector/276-mnl.pdf)
- Canberra/MIRION带前放的PMT
    - [Model 2007/2007P Photomultiplier Tube Base/Preamplifier](http://wuhongyi.cn/HardwareNote/pdf/Detector/Model-2007-2007P-SS-CSP0071.pdf)
- ET-Enterprises公司PMT设计说明
	- http://www.et-enterprises.com/
    - [design of PMT output ciruits](http://wuhongyi.cn/HardwareNote/pdf/Detector/rp065_design_of_PMT_output_ciruits.pdf)
- Photonis产品列表
	- [Photomultiplier Tubes Catalogue](http://wuhongyi.cn/HardwareNote/pdf/Detector/PhotonisCatalog.pdf)


## PMT详细产品说明

- [HAMAMATSU / PHOTOMULTIPLIER TUBES Basics and Applications](http://wuhongyi.cn/HardwareNote/pdf/Detector/pmt_hand_book_complete.pdf)
- [HOW TO USE PHOTOMULTIPLIER TUBES AND PERIPHERAL CIRCUITS](http://wuhongyi.cn/HardwareNote/pdf/Detector/PMT_handbook_v3aE-Chapter5.pdf)
	- P11  在倒数两极加阻尼器，会导致上升时间变慢但是下降部分的震荡大大减小。

带前放一方面减小输出阻抗，另一方面适合较远距离的传输。


preamplifiers – the use of a preamplifier must be considered in those applications where the photomultiplier is separated from the data acquisition system by many metres of cable. Unless properly terminated, the transmission cable will introduce pulse distortion and reflections into the system. Charge sensitive preamplifiers perform the function of charge-to-voltage-conversion, while providing a low impedance output suitable for driving long cables. They are often used in conjunction with a shaping or main amplifier and the option of a preamplifier incorporated into a tube base is offered by several manufacturers.

The difficulties associated with fast photomultiplier pulses, where current saturation is a very real problem, have now been considerably reduced by the introduction of high speed pulse amplifiers in integrated or hybrid form. Their compact construction allows for convenient location close-up to the anode of the photomultipier. 

----


文献：

- 2006
	- [NIMA / New Photonis XP20D0 photomultiplier for fast timing in nuclear medicine](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-S0168900206008643-main.pdf)



<!-- PMT.md ends here -->
