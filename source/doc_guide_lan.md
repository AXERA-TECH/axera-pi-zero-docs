# GPIO/I2C/SPI等通讯接囗操作示例

## 对GPIO的读写操作

1.在控制台使用echo命令将要操作的GPIO编号
```
echo N > /sys/class/gpio/export	  //export之后就会生成
/sys/class/gpio/gpioN 	目录
```

2.在控制台使用echo命令设置GPIO方向
```
echo in > /sys/class/gpio/gpioN/direction
echo out > /sys/class/gpio/gpioN/direction 	
```

3.在控制台使用cat或echo命令查看GPIO输入值或设置GPIO输出值
```
echo N > /sys/class/gpio/export	  //export之后就会生成
/sys/class/gpio/gpioN 	目录
cat /sys/class/gpio/gpioN/value	 //查看输入值
echo 0 > /sys/class/gpio/gpioN/value  //输出低
echo 1 > /sys/class/gpio/gpioN/value  //输出高
```
```
例如，设置GPIO1_17方向：
echo 49 > /sys/class/gpio/gpioN/export
echo in > /sys/class/gpio/gpio49/direction //输入使能
cat /sys/class/gpio/gpio49/value  //查看输入值
echo out > /sys/class/gpio/gpio49/direction  //输出使能
echo 0 > /sys/class/gpio/gpio49/value  //输出低
echo 1 > /sys/class/gpio/gpio49/value  //输出高
cat /sys/class/gpio/gpio49/direction  //查看GPIO方向GPIO的电平值只有0和1。0为低电平，1为高电平。
```

4.在控制台使用echo命令将操作的GPIO编号unexport
```
echo N > /sys/class/gpio/unexport
```

GPIO分为#0、#1、#2、#3，每组有32个GPIO。做如下约定N为GPIO的编号，P为组号取值范围为0、1、2、3，可以得到N=p*32+offset。
以GPIO1_17为例计算GPIO的编号，可以知道P=1，offset为17，N=1*32+17=49。