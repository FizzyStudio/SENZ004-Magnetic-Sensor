# SENZ004 数字贴片磁感应传感器


### 概述

> 基于感磁材料的磁性传感器，可以用来对磁性材料（磁铁）的探测，探测范围可达3cm左右(探测范围和磁性强弱有关)，与Arduino专用传感器扩展板结合使用，可以制作与磁性材料（磁铁）相关的互动作品。

### 技术规格

* 工作电压：+3.3/5V
* 接口类型：数字
* 输出信号：平时输出高电平，检测到磁性时输出低电平
* 重量：5g

### 引脚定义

> 数字磁感应传感器模块管脚定义：
  1 信号输出
  2 电源(VCC)
  3 地(GND)

### 连接示意图


### 示例代码

    int ledPin = 13;                // choose the pin for the LED
    int inputPin = 2;               // choose the input pin  
    int val = 0;                    // variable for reading the pin status
    void setup() {
      pinMode(ledPin, OUTPUT);      // declare LED as output
      pinMode(inputPin, INPUT);     // declare pushbutton as input
    }
    void loop(){
      val = digitalRead(inputPin);  // read input value
      if (val == HIGH) {            // check if the input is HIGH
        digitalWrite(ledPin, LOW);  // turn LED OFF
      } else {
        digitalWrite(ledPin, HIGH); // turn LED ON
      }
    }
  
  ### 更多
  
