##### 1、U26的VREF_DAC改成VREF_ADC；

##### 2、R217、R231、R245、R259的VDD_5V_MAIN改成VREF_ADC；

##### 3、R212、R222、R226、R236、R240、R250、R254、R264改成51K；

##### 4、R215和R216等改成0欧；

##### 5、R217等改成1K；

##### 6、R218、R220、R221等改成1.5K；

##### 7、FB1去掉，U25焊上REF3025AIDBZR； 

##### 8、U25改用3.3V供电；

##### 9、D21 pin1的GND改成；

##### 10、R162和R168由原来的887R改成1.1K，15V改成12V电源

##### 11、由于FPGA 5M240ZT100资源不够，所以改用5M570ZT100，但有部分脚不兼容：

###### 		1）39pin由原来的F_EX_DATA5改接到1.8V，26pin由原来的NC接到F_EX_DATA5；

###### 		2）88pin EX_RD 	--> 1.8V, 98pin NC	-->EX_RD;

###### 		3)8pin NC 	-->GND;

###### 		4)1pin	GNG	-->NC;

###### 		5)90pin EX_ADD0	-->GND, 99pin NC	-->EX_ADD0;

###### 		6)95pin EX_ADD3	-->GND, 100pin NC	-->EX_ADD3;

###### 7）37pin  F_EX_DATA2 -->,   27pin NC -->F_EX_DATA2 ;

​		