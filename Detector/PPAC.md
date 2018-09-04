<!-- PPAC.md --- 
;; 
;; Description: 
;; Author: Hongyi Wu(吴鸿毅)
;; Email: wuhongyi@qq.com 
;; Created: 一 9月  3 23:27:44 2018 (+0800)
;; Last-Updated: 二 9月  4 10:43:22 2018 (+0800)
;;           By: Hongyi Wu(吴鸿毅)
;;     Update #: 8
;; URL: http://wuhongyi.cn -->

# PPAC


[Parallel plate avalanche counter(PPAC) development and performance test for Rare Isotope Science Project(RISP)](http://wuhongyi.cn/HardwareNote/pdf/Detector/ppac_for_risp.pdf)



文献：


- 1976
	- [NIM / A LARGE AREA PARALLEL PLATE AVALANCHE COUNTER](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-0029554X76904237-main.pdf)
- 1979	
	- [NIM / A SQUARE METER POSITION SENSITIVE PARALLEL PLATE DETECTOR FOR HEAVY IONS](http://wuhongyi.cn/HardwareNote/pdf/article/1-s2.0-0029554X79900831-main.pdf)
- 2017	
	- [Construction and Performance Test of Prototype Parallel Plate Avalanche Counters at RAON](http://wuhongyi.cn/HardwareNote/pdf/article/risp-ppac.pdf)


----

## structure

- 10 MΩ (600-800V)
- 220 pF
-  Mylar of 2~3.5 µm
- Need pure quenching gas of C4H10(W = 23.7 eV), C3F8(W = 34.4 eV)

Read out avalanche signals from anode and cathode; Anode for time & triggering, cathode for position measuremen


## Delay line readout

- 0603 chip inductor 91 nH (2% tolerance)
- 0603 chip capacitor 39 pF (1% tolerance)
- 0603 chip resistor, 500 kΩ




<!-- PPAC.md ends here -->
