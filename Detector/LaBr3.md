<!-- LaBr3.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 二 6月  6 14:23:24 2017 (+0800)
;; Last-Updated: 三 6月  7 23:10:39 2017 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 8
;; URL: http://wuhongyi.cn -->

# LaBr3

关于PSD [Enhanced α-γ Discrimination in Co-doped LaBr 3 :Ce](http://wuhongyi.cn/HardwareNote/pdf/Detector/enhanced_a-g_discrimination_in_co-doped_labr3_ce.pdf)


3英寸探头，型号KLB7676。高压+600V，漏流0.27mA。负信号，噪声在正负0.5mV，上升时间40ns，下降时间60+ns。


----

## DT5730测试

源
- Cs137 0.662MeV
- Co60 1.17/1.33 MeV

高压加到+600V

获取参数：波形记录2048个点，PreTrigger1000个点。阈值8300，DC Offset-40

通过QDC积分得到能量。
看到奇怪的现象，峰的右边有拖尾。


<!-- LaBr3.md ends here -->
