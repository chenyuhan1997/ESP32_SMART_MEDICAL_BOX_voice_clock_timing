# ESP32_SMART_VOICE_ALARM_PWM_LIGHT
The main function here is to set the alarm clock through the WEB terminal, and then you can control the servo, voice, and buzzer regularly, and set the button to close. In order to achieve multi-threading, the FreeROST system is used, and dual-core is used.

English version：

Something you should know:
A. The list of materials I used for this design is as follows:
	1. ESP-WROOM-32(ESP32 DEVKIT V1)
	2. a normal buzzer
	3. 0.91 inch oled (IIC and SSD1306)
	4. Mini Servo SG90 9g Servo 
	5.LM386
	6.a normal speaker
B. I use the FreeRost and ESP32 inherits this operating system, so you can delete some head file
C. I use the cheaper plan about the voice part, you can use a file of MP3, convert MP3 to WAV(Sampling rate < 16000);
    and copy by C to your sound.h
  （Software: Audacity and HxD）
D. if you have some question about it ,you can contact me by CSDN

MY CSDN NAME: Reedsway在重庆


中文介绍：
我这个设计其实很简单，就是一个ESP32的智能药箱。具体的操作就是网络端指令，控制舵机，语音和蜂鸣器。
并且可以WEB端进行定时的功能。没有采用SPIFFS异步服务器，其实更好理解。我每一行都有中文注释。非常详细。
可以帮助你对ESP32的部分功能充分了解。再者，我这个设计，用了FREEROST，采用了双核。

本次用到的材料非常廉价：淘宝的ESP-WROOM-32, 一个SG90舵机，一个蜂鸣器，一个LM386功放，
一个喇叭大概就这些，还有些按键啥的，0.91寸OLED。

其中的难点，我觉得主要是语音那部分。因为想要廉价的语音播放，所以这面直接使用了转码的形式（有点弱智）
这里面先将MP3转为WAV（采样率在16000之下），然后再复制成C语言就行了。
用到的软件是：Audacity和HxD

具体其他可以咨询我的CSDN
