# BluetoothJoystick-Blog
This is the blog about our Eklavya Mentorship Project, Bluetooth Joystick.A wireless joystick with ESP-32 microcontroller and Dual Axis Joystick Module using the Bluetooth connectivity.

<!-- ABOUT THE PROJECT -->
## About The Project
### Aim 
The aim of this project is to make a Bluetooth Joystick using ESP32 which establishes Bluetooth Low Energy (BLE) Connection with the host device to provide controls by providing inputs. The ESP32 is capable of getting a unique signal for each key press. Accordingly it will transmit the signal information over bluetooth to the host device.

### This image is the illustration of our hardware.
![Hardware](https://user-images.githubusercontent.com/84867886/137713259-8dfb6e91-b3af-45e9-91c0-fc0ee07c7167.jpeg)
 

## Domains of the Project
In this project, we study the ESP-IDF framework, which is for the esp-32. The framework has some exclusive features and functions which enable the esp-32 of its vast reach. Espressif's official IoT Development Framework for the ESP32, ESP32-S, and ESP32-C series of SoCs is a boon to the embedded world. It provides a self-sufficient SDK for any generic application development on these platforms, using programming languages such as C and C++.
![ESP-IDF](https://github.com/Krishna-13-cyber/BluetoothJoystick-Blog/blob/main/esp-idf)
FreeRtos is another domain that plays a vital role in embedded systems, which is used as the real-time operating system for microcontrollers that makes small, low-power edge devices easy to program, deploy, secure, connect, and manage.FreeRTOS) is an operating system for microcontrollers that makes small, low-power edge devices easy to program, deploy, secure, connect, and manage.
![Free-Rtos](https://github.com/Krishna-13-cyber/BluetoothJoystick-Blog/blob/main/freertos.jpeg)
We also get to know about the wireless connections especially Bluetooth in this project. The range, its transmission efficiency, the level of modification, advancement, and upgrade with each version of BlueTooth connectivity. In this project, the emphasis is on making a wireless setup,
ESP-32 has the feature of BlueTooth connectivity which has the version v4.2.To start off we connect the esp-32(microcontroller) as a mouse and give it a basic functionality that on the press of any key on the keyboard, the cursor according to the condition of the code will go up or down.

## Some Stimulating Stuff in Store
Bluetooth Joystick!
Controller or a Joystick! Yes we might have came across at least once in our lifetimes. But the simplicity felt in using it was the exact opposite when we got started to make it. But the odds were with us as the project was under the Eklavya Mentorship. Which means the project was not only a product of our hardworking, research and dedication but also of the experience and guidance of our mentors Gautam and Dhairya who made sure we were on the right track. Getting back to the project, we started the project by familiarising ourselves with what we were getting into. So the initial stage was all about research and learning about all the Bluetooth terminologies as we aimed to make it wireless and nothing better than Bluetooth for the easiest connection of the master and slave devices.We learned about the range, its transmission efficiency, the level of modification, advancement, and upgrade with each version of BlueTooth connectivity We moved on to the ESP-IDF Framework as the heart of our project was ESP-32. Now, why ESP-32? Why not something else? Well the project will speak for itself, give it a read till the end!
Espressif's official loT Development Framework for the ESP32, ESP32-S, and ESP32-C series of SoCs is a boon to the embedded world and makes the coding easier as against Arduino IDE.It provides a self-sufficient SDK for any generic application development on these platforms by using programming languages such as C and C++.This was crucial for combining the wireless communication along with embedding the code into our joystick.
The operating system which we implemented was FreeRTOS. FreeRTOS is another domain that plays a vital role in embedded systems, which is used as the real-time operating system for microcontrollers that makes small, low-power edge devices easy to program, deploy, secure, connect, and manage.
After a few weeks of soaking in the required information ,we headed towards the hardware part.
We learnt about the various connections, played with a few circuits on the breadboard. It was also essential to learn about the GPIO System of the ESP-32. 
With all this done, we came down to the part where we actually had to Embed the code into the ESP-32.
We started out with the normal blink test with the ESP-32. And also started to learn the code structure of the various Bluetooth API’s and implement it. 
Gradually setting up the Bluetooth part of our Joystick, we tested it out by connecting our Joystick to the ESP-32 as HID-Mouse and HID-Keyboard.
For this we needed to connect our Joystick with the ESP-32 in such a way that there shouldn’t be any mistakes made while connecting the wires/jumpers. 
<!-- GETTING STARTED -->
## Getting Started
### Prerequisites
To flash this project install ESP-IDF: https://github.com/espressif/esp-idf
### Cloning the repository
Clone the project by typing the following command in your Terminal/CommandPrompt
```
git clone https://github.com/Krishna-13-cyber/BluetoothJoystick.git

cd BluetoothJoystick
```

## Hardware
### Connections
Connect the ESP32 to your desktop via USB to flash the code in it. And connect the Joystick to ESP32 as per the table given below.
![Connection Illustration](https://user-images.githubusercontent.com/84867886/137712945-33cc0423-3b61-4909-b2e1-0d28a778a47f.png)
JoyStick Pin | ESP32 Pin
--------- | -----------
5V | 3V3
GND | GND
VRx | GPIO39
VRy | GPIO34
SW | GPIO25

You are all set to flash the code after completing the connections.
## Usage
After following the above steps , use the following commands to:
Build
```
idf.py build
```
Flash
```
idf.py -p (PORT) flash monitor
```
Configuration

```
idf.py menuconfig
```

## Code Flowchart
![Flowchart](https://user-images.githubusercontent.com/84867886/138583223-d8353de8-228b-41de-8cc5-d18d5cb22d7a.png)

## Results and Demo
These are the output obtained in initial stage as shown in the link attached to the below mentioned video.
* [ADC Values](https://drive.google.com/file/d/1rm1N4SgXiCJK_13tnsdQ1i77aFfMDrW-/view?usp=sharing)
* [Movement of Cursor by Joystick](https://drive.google.com/file/d/1VwI7GT10AZU_PWkB9DNiD4OaYqe5EC_o/view?usp=sharing)

These are the Output of the Games played with help of Joystick Module.
![Mouse-Game](https://github.com/Krishna-13-cyber/BluetoothJoystick/blob/main/docs/MouseGame.gif)
![Mouse-Game2](https://github.com/Krishna-13-cyber/BluetoothJoystick/blob/main/docs/Game2.gif)
<!-- FUTURE WORK -->
## Future Work
* The following developments are yet to be achieved
- [x] Establishing BlueTooth Connection
- [x] Obtaining ADC Values
- [x] Moving the Cursor 
- [x] Controlling a Game
- [ ] Using it to send keyboard keys
- [ ] Adding more buttons to it


## Contributors
* [Krishna Narayanan](https://github.com/Krishna-13-cyber)
* [Om Sheladia](https://github.com/omsheladia)

## Acknowledgements and Resources
* [SRA-VJTI for providing this wonderful opportunity](https://sravjti.in/) Eklavya 2021 
* Special thanks to [Gautam Agrawal](https://github.com/gautam-dev-maker)
* Special thanks to [Dhairya Shah](https://github.com/dhairyashah1) 
* https://github.com/nkolban/esp32-snippets
* [Krishna's Notes](https://docs.google.com/document/d/1IP-aztx2PFOdQ0YAVJ_k0vlUyVbuh3PO7OZ1GM7nCuU/edit?usp=sharing)
* [Om's Notes](https://docs.google.com/document/d/1GOzxKsOPQXyTHjrb4r8Ifgxr5I2fEamjWZOJTkD3TnQ/edit?usp=sharing)

## License
The [License](https://github.com/Krishna-13-cyber/BluetoothJoystick/blob/main/LICENSE) Used for this Project.

Happy Blogging!!!
