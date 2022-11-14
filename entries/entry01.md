# Entry 1
##### 11/9/2022

# Wiring
I started by trying to create a glove that could recognize my finger movements. To start, I drafted up an idea of how the gloves would look like on my hands. I searched up wiring diagrams for the flex sensors and then directly wired it to the gloves. It confused me when the flex sensors would either report 0 or 4095. The reason was it was either not powered, or not grounded. If it was powered but not grounded, it would read 4095. If it wasn't powered, it would read 0. Understanding the difference between the pins on the Arduino was the hardest part. There were GPIO pins, and then there were GPIO pins that supported ADC.

# Google

I started by looking up [basic wiring diagrams for the Arduino and flex sensors](https://lastminuteengineers.b-cdn.net/wp-content/uploads/arduino/Wiring-Flex-Sensor-To-Arduino.png), but I had no idea how to use the resistors or the precrimped jumper wires that I had, nor did I have any idea on how to verify if my code was working. So I had to install the Arduino IDE. It frustrated me to no end that the ESP32 had so many variations, and it was not documented which ESP32 I had. So that meant that I had to manually upload it for each ESP32 that was in the library. Compiling was extremely slow and it was time consuming. After I finally got it working, and voila, it read. Issue is... it was inaccurate at best, completely wrong at worst.

# EDP

I am currently on step 5 of the EDP. I am currently working towards creating a viable prototype. The wiring works and I only have to write something that could interpret the hand signs. I would then try to translate the hand signs to images, then it should translate that image to the corresponding word.

# Skills

Skills that I've used are "How to learn" and "How to Google". Starting this project, I had no idea how to start with researching what I needed to learn. So I started with looking up wiring tutorials. I learned how to wire an Arduino and how to flash them.


[Next](entry02.md)

[Home](../README.md)
