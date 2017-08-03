# SENZ004 Digital Magnetic Sensor

### Introduction

> what's the best way to detect the magnet? Use anther magnet. But it's not sensitive enough. You have to feel it by youself.Right.This magnetic sensor knows whether there is a magnetic object nearby or not. And it correctly tells you through ditigal output.See below picture for a quick demo! 

### Specification

* Supply Voltage: 3.3V to 5V
* Indicator LED on board
* Interface: Digital
* Size:22x30mm

### Connection Diagram


### Sample Code

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
 
 ### more
    
