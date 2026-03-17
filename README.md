# 8051 LED Blink

## 📌 Description
This project demonstrates how to blink an LED using AT89C51 microcontroller.

## 🛠 Tools Used
- Proteus (Simulation)
- Keil uVision (C Programming)

## 🔌 Components Required
- AT89C51 Microcontroller
- LED
- Resistor (220Ω)
- Power Supply

## ⚙️ Working Principle
The LED is connected to Port 1 of the microcontroller.  
The program continuously turns the LED ON and OFF with a delay, creating a blinking effect.

## 💻 Program Code
```c
#include <reg51.h>

void delay()
 {
    int i, j;
    for(i=0; i<ms; i++)
    for(j=0; j<1000; j++);
}

void main()
{
    while(1)
 {
        P1 = 0xFF;   // LED GLOWS
        delay();
        P1 = 0x00;   // LED TURNS OFF
        delay();
    }
}

## ▶️ Output
LED blinks continuously

## 📷 Circuit Diagram
![Circuit](circuit.png)

