In this Quick Start guide we'll connect the SparkFun OLED Display (1.5in., 128x128) to a SparkFun IoT RedBoard - ESP32 and use the SparkFun Qwiic OLED Arduino library to produce a rotating cube on the display.

<figure markdown>
[![Short video showing cube demo on the OLED](./assets/img/Qwiic_OLED_1.5-Cube.gif){ width="600"}](./assets/img/Qwiic_OLED_1.5-Cube.gif)
</figure>

If you're not familiar with using breakout and development boards or the Arduino IDE, refer to the [Hardware](./hardware_overview.md) & [Software](./arduino_setup.md) sections for a detailed overview of the board along with instructions on soldering to and connecting the breakout, installing and using the SparkFun MY1690X MP3 Decoder Arduino Library.

## Basic Assembly

With the Qwiic Ecosystem all you'll need to do to assemble the Qwiic OLED - 1.5" is the following steps:

* Connect the Qwiic OLED Display to the RedBoard IoT - ESP32 using a Qwiic cable.
* Connect the RedBoard IoT - ESP32 to your computer with a USB-C cable.

<figure markdown>
[![Completed Qwiic assembly](./assets/img/Qwiic_OLED_1.5-Assembly.jpg){ width="600"}]
</figure>

## Arduino Example

Let's move on to installing the SparkFun Qwiic OLED Arduino library (and boards packages if needed) to . Follow these steps to upload and run the "Cube" example.

* Install the SparkFun Qwiic OLED Arduino library using the [library manager](https://docs.arduino.cc/software/ide-v2/tutorials/ide-v2-installing-a-library/) by searching for "SparkFun Qwiic OLED".
* If you don't already have the RedBoard IoT - ESP32 board definition installed, you'll need to install the "esp32" boards package by Espressif Systems. Copy this JSON URL: <code>https://espressif.github.io/arduino-esp32/package_esp32_dev_index.json
</code> to the "Additional Boards Manager URLs" in the "Preferences" menu and then search for "esp32" in the [boards manager](https://docs.arduino.cc/software/ide-v2/tutorials/ide-v2-board-manager) tool and install the latest version of the "esp32 by Espressif Systems" boards package.
* Open "Example-07_Cube" from the SparkFun Qwiic OLED Arduino library folder. Comment out the line for the Qwiic Micro OLED and uncomment the line for the Qwiic 1.5" OLED like the code below:

``` c++
//QwiicMicroOLED myOLED;
//QwiicTransparentOLED myOLED;
//QwiicNarrowOLED myOLED;
//Qwiic1in3OLED myOLED;
Qwiic1in5OLED myOLED;
```

* Select your Board and Port and click the "Upload" button.

Once the code finishes compiling and uploading, the OLED should display a rotating cube similar to the video below:

<figure markdown>
[![Short video showing cube demo on the OLED](./assets/img/Qwiic_OLED_1.5-Cube.gif){ width="600"}](./assets/img/Qwiic_OLED_1.5-Cube.gif)
</figure>

This example has plenty of variables we can adjust to change things like the size, location and rotation speed of the cube. For the video above, we doubled the size of the cube to make it easier to see. Try playing around with the different variables and re-uploading it to change the appearance and movement of the cube.