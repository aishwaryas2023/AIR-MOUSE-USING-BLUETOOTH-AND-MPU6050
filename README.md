# AIR-MOUSE-USING-BLUETOOTH-AND-MPU6050

## Overview
This project implements an **Air Mouse** that allows users to control a computer cursor using hand gestures instead of a traditional mouse. It uses an **ESP32 microcontroller** with built-in Bluetooth and an **MPU6050 motion sensor** (accelerometer + gyroscope) to detect motion and orientation. The ESP32 processes the sensor data and sends corresponding cursor commands to a computer, emulating a standard Bluetooth mouse.

This creates a portable, wireless, and intuitive input device for presentations, gaming, virtual reality, and accessibility applications.

---

## Features
- Real-time cursor control using hand gestures  
- Wireless communication via Bluetooth  
- Gesture-based click detection (optional)  
- Smooth cursor movement with filtering techniques  
- Compact and portable design  

---

## Applications
- Move slides or cursor during presentations without touching a laptop  
- Gesture-based gaming interaction  
- Remote control for smart devices and media systems  
- Virtual reality motion detection  
- Accessibility: helps users with limited mobility  
- Learning and prototyping sensors, Bluetooth, and gesture-based control  

---

## System Design

### Hardware Components
- ESP32 Development Board: Main controller with Wi-Fi and Bluetooth  
- MPU6050 Sensor: 3-axis accelerometer + gyroscope for motion detection  
- Optional: LDR for click detection, buttons, SPDT switch, Velcro ties, TP4056 charging module  
- Power Supply: Li-ion battery or USB  
- Connecting Wires, Breadboard, Perfboard  

### Software Components
- Arduino IDE for programming  
- Libraries: MPU6050, Wire, Bluetooth HID, etc.  
- Serial Monitor for testing and debugging  

### Architecture
1. **Sensing Movement:** MPU6050 detects hand motion and tilt  
2. **Processing Data:** ESP32 converts sensor readings into cursor movements  
3. **Wireless Communication:** ESP32 sends data via Bluetooth to the computer  

---

## Implementation
The MPU6050 is connected to the ESP32 via I2C pins. The sensor detects hand movements and sends data to the ESP32. The ESP32 processes this data and sends corresponding cursor movement signals to the computer via Bluetooth. Optional LDR or buttons can be used to detect click actions.  

A custom PCB or breadboard can be used for hardware setup, providing stability, reducing wiring issues, and making the system more compact and portable.  

---

## Results
- Smooth, real-time cursor movement using hand gestures  
- Reliable Bluetooth communication  
- Custom PCB improved stability and reduced signal noise  
- Portable, low-cost, and easy-to-use device  
- Minor calibration may be required for different users’ hand movement speeds  

---

## Conclusion
The Air Mouse using ESP32 successfully demonstrated that motion sensing and wireless communication can create a simple and effective alternative to a traditional mouse. The MPU6050 sensor accurately captured hand movements, and the ESP32 provided smooth, real-time cursor control.  

Using a custom PCB improved stability, reduced wiring issues, and made the device compact and robust. Overall, this project achieved its goals of building a low-cost, portable, and intuitive gesture-based mouse.  

---

## Future Work
- Gesture recognition for clicking, scrolling, and zooming  
- Advanced sensors for higher accuracy and less drift  
- Rechargeable battery with USB charging  
- Power-saving sleep mode for longer battery life  
- Ergonomic 3D-printed or custom enclosure  
- Multi-platform support (Windows, macOS, Linux, Android)  
- Integration with voice control
