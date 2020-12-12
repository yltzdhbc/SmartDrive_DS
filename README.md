# SmartDrive_DS
智驱 总线舵机/pwm舵机 一体化驱动控制器（SmartDrive Digital Servo）

> 773673787@qq.com



![SmartDrive_BDCM2_Front](img/SmartDrive_DS_3.jpg)



**综述**

该驱动是 **智驱系列** 的串口总线舵机版本，该版本具有3个串口总线舵机接口，支持博创CDS55XX系列舵机、Robotics的Dynamixel系列总线舵机，使用单线半双工串口，1M的波特率，波特率可调。支持8路PWM舵机可轻松驱动普通50HZ的PWM舵机，且PWM分辨率达到了1/2000，控制更精准。支持更改PWM周期，可配置为330HZ以用于相应速度更快的数字舵机。对于PWM舵机内置了速度斜坡，速度限制等，以获取更平稳的运动。



**功能**

- 支持舵机：博创CDS55XX系列、Robotics Dynamixel系列、普通PWM舵机、数字PWM舵机。
- 通信能力：最高1M波特率串口半双工总线，DMA接收。
- 最多支持：最多253个总线舵机、8个PWM舵机。
- 控制方式：CAN总线、USART串口
- 控制协议：SmartDrive SDK



**硬件参数**

| 元件         | 型号            | 说明                           |
| ------------ | --------------- | :----------------------------- |
| 处理器       | GD32F103CBT6    | 20KRAM 128K FLASH 72MHZ        |
| 串口逻辑     | SN74HC126       | 具有三态输出的四路总线缓冲器闸 |
| CAN收发器    | TJA1051         | 最高1M HZ 可选则的120R电阻     |
| 总线舵机接口 | XH2.54-WI-3P    | 总线舵机接口                   |
| PWM接口      | HRD2.54-LI-3P   | 3p舵机接口                     |
| 用户交互接口 | KF2EDGR-3.81-9P | 高品质3.81接口                 |



**通信方式**

- CAN总线，使用SmartDrive SDK可以快速的集成到系统中，使用起来非常方便。
- *USART*（串口），默认115200通信速率，使用SmartDrive SDK。
- USB，使用VCP协议直接连接电脑，与上位机进行通信，可直接对控制器进行调试，配置参数。



**SmartDrive SDK**

SmartDrive SDK是专为SmartDrive系列驱动器开发的通信协议，支持CAN 和 USART两种方式通信，现主要支持STM32 F1、F4系列，使用HAL库。

为了使SmartDrive系列驱动的开发变得简单，自带了很多例程，对通信协议部分做了单独的解耦合，确保使用HAL库的用户可以很轻松的移植上手。 

![](img/uptech_protocol.pdf_page_01.jpg)
![](img/uptech_protocol.pdf_page_02.jpg)
![](img/uptech_protocol.pdf_page_03.jpg)
![](img/uptech_protocol.pdf_page_04.jpg)
![](img/uptech_protocol.pdf_page_05.jpg)
![](img/uptech_protocol.pdf_page_06.jpg)
![](img/uptech_protocol.pdf_page_07.jpg)
![](img/uptech_protocol.pdf_page_08.jpg)
![](img/uptech_protocol.pdf_page_09.jpg)
![](img/uptech_protocol.pdf_page_10.jpg)
![](img/uptech_protocol.pdf_page_11.jpg)
![](img/uptech_protocol.pdf_page_12.jpg)
![](img/uptech_protocol.pdf_page_13.jpg)

![SmartDrive_BDCM2_Front](img/SmartDrive_DS_4.jpg)
![SmartDrive_BDCM2_Front](img/SmartDrive_DS_2.jpg)
![SmartDrive_BDCM2_Front](img/SmartDrive_DS_3.jpg)
![SmartDrive_BDCM2_Front](img/SmartDrive_DS_5.jpg)
![SmartDrive_BDCM2_Front](img/SmartDrive_DS_1.jpg)