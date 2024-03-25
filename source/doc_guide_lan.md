# GPIO/I2C/SPI 等通讯接囗操作示例

## GPIO 读写操作

1.在控制台使用 `echo` 命令将要操作的 GPIO 编号

```
echo N > /sys/class/gpio/export	  //export之后就会生成
/sys/class/gpio/gpioN 	目录
```

2.在控制台使用 `echo` 命令设置 GPIO 方向

```
echo in > /sys/class/gpio/gpioN/direction
echo out > /sys/class/gpio/gpioN/direction 	
```

3.在控制台使用 `cat` 或 `echo` 命令查看 GPIO 输入值或设置 GPIO 输出值

```
echo N > /sys/class/gpio/export	  //export之后就会生成
/sys/class/gpio/gpioN 	目录
cat /sys/class/gpio/gpioN/value	 //查看输入值
echo 0 > /sys/class/gpio/gpioN/value  //输出低
echo 1 > /sys/class/gpio/gpioN/value  //输出高
```

```
例如，设置 GPIO1_17 方向：
echo 49 > /sys/class/gpio/gpioN/export
echo in > /sys/class/gpio/gpio49/direction //输入使能
cat /sys/class/gpio/gpio49/value  //查看输入值
echo out > /sys/class/gpio/gpio49/direction  //输出使能
echo 0 > /sys/class/gpio/gpio49/value  //输出低
echo 1 > /sys/class/gpio/gpio49/value  //输出高
cat /sys/class/gpio/gpio49/direction  //查看GPIO方向GPIO的电平值只有0和1。0为低电平，1为高电平。
```

4.在控制台使用 `echo` 命令将操作的 GPIO 编号 unexport

```
echo N > /sys/class/gpio/unexport
```

GPIO 分为 #0、#1、#2、#3，每组有 32 个 GPIO。做如下约定：N 为 GPIO 的编号，P 为组号取值范围为 0、1、2、3，可以得到 N=px32+offset。以 GPIO1_17 为例计算 GPIO 的编号，可以知道 P=1, offset 为 17，N=1x32+17=49