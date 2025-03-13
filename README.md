# PCB_Design

  Some of my privite PCB design projects.
#1: CH340, FT232, and CP2102 Breakout boards 
  All of these are USB-to-UART converters, but with an enhanced feature: built-in ESD protection. Most converters on the market lack this protection, making them vulnerable to damage if accidentally touched with charged static hands. With  ESD protection, My redesign for devices offered greater durability and reliability.
  
#2: Mult I2C Devices
  The MCu "ESP32" typically struggles to interface with multiple I2C devices that share the same address, such as OLED displays and sensors, making direct communication impossible. My design solves this issue by integrating an I2C multiplexer, allowing the ESP32 to switch between multiple devices with identical addresses seamlessly.
The multiplexer has 8 I2C channels, and in this design, I used two multiplexers to manage multiple TOF sensors efficiently. The ESP32 controls the multiplexers, switching between I2C channels as needed to ensure smooth operation.

#3: USB to RF 2.4GHz Convertor
This design utilizes an STM32L4 USB interface and an nRF24L01 2.4GHz module to establish a wireless connection between two hosts over a distance of more than 100 meters. To enhance coverage, the design includes an external SMA antenna connector, ensuring a wider and more reliable communication range.
  
