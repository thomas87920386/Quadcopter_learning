The ".ino" file is the Arduino script used to communicate with the IMU, MPU6050. In this case, the total practice will be divided into two sections: one to read and show the measurement value in the Arduino serial monitor and the second to calibrate the IMU measurement.

Before the first section, the sensor needs to connect to the MCU. At this time, some points need to be checked. One is the meaning of the IMU pin, and choosing which pin will be used for the specific function, such as the gyroscope or the accelerometer. Next, finding the pin at the MCU should be connected to the IMU. In this folder, the practice will focus on the gyroscope function in the IMU so that the pin will be chosen for the gyroscope at first. The MPU6050 mains to use the I2C protocol for transmission, so two pins need to be used "SDA", and "SCL". "SDA" is for serial data, and the "SCL" is for serial clock. Finally, the sensor needs power, so the "VCC" and "GND" need to be used. 

After deciding on the pin at the IMU, the next is to decide on the pin at the MCU. In the previous section, the pins used in the IMU are "VCC", "GND", "SDA", and "SCL", so the corresponding pins in the MCU are "+5V", "GND", "A4", and "A5" in the MCU, Arduino nano board. The following schematic diagram shows the reason why to use the "A4" and "A5" for "SDA", and "SCL".
![image](https://github.com/user-attachments/assets/baf2eb29-a883-459c-86d5-c8094efff349)


