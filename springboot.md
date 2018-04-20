# <p align = "center">springboot - 2.0.1</p> #
# 4、springboot 的特征 #
#### 23、SpringApplication ####
#### 24、外部配置文件 ####
##### &nbsp;&nbsp;&nbsp;&nbsp;24.1、配置随机数 #####


> The RandomValuePropertySource is useful for injecting random values (for example, into secrets or test cases). It can produce integers, longs, uuids, or strings, as shown in the following example:

	my.secret=${random.value}  //
	my.number=${random.int}
	my.bignumber=${random.long}
	my.uuid=${random.uuid}
	my.number.less.than.ten=${random.int(10)}
	my.number.in.range=${random.int[1024,65536]}
>The random.int* syntax is OPEN value (,max) CLOSE where the OPEN,CLOSE are any character and value,max are integers. If max is provided, then value is the minimum value and max is the maximum value (exclusive).