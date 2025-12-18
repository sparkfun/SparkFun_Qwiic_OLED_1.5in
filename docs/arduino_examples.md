Let's take a look at a few of the examples included in the SparkFun Qwiic OLED Arduino Library

## Example 01 - Hello

The first example in the Qwiic OLED library shows the basic setup of the library and generates a simple text display of "Hello". Open the example by navigating to **File** > **Examples** > **SparkFun Qwiic OLED Arduino Library** > **Example-01_Hello**. All the examples included in the library work with the five supported Qwiic OLEDs with a simple adjustment to a couple lines in the start of the sketch. The examples default to select the Qwiic Micro OLED so we need to adjust the definition to switch to the 1.5" OLED. Comment out the line for the Qwiic Micro OLED and uncomment the line for the Qwiic 1.5" OLED like the code below:

``` c++
//QwiicMicroOLED myOLED;
//QwiicTransparentOLED myOLED;
//QwiicNarrowOLED myOLED;
//Qwiic1in3OLED myOLED;
Qwiic1in5OLED myOLED;
```
After selecting the correct OLED, select your Board and Port and click the "Upload" button. Once the code finishes uploading the display should initialize and display a static text print saying "Hello" like the photo below:

<figure markdown>
[![Photo of the Qwiic OLED 1.5 displaying "Hello"](./assets/img/Qwiic_OLED_1.5-Hello.jpg){ width="600"}](./assets/img/Qwiic_OLED_1.5-Hello.jpg "Click to enlarge")
</figure>

## Example 02 - Shapes

The second example demonstrates various methods for drawing shapes using the library. Open the example by navigating to **File** > **Examples** > **SparkFun Qwiic OLED Arduino Library** > **Example-02_Shapes**. Remember we need to adjust the code to work with the OLED 1.5" so make sure to adjust the definitions like we did for Example 01 before uploading. After adjusting the OLED definition, click the "Upload" button. Once the code finishes uploading, the display will initialize and start drawing various shapes using different drawing methods to create various types of lines, rectangles and circles like the video below shows:

<figure markdown>
[![Short video showing the Qwiic OLED 1.5 displaying various shapes and lines](./assets/img/Qwiic_OLED_1.5-Shapes.gif){ width="600"}](./assets/img/Qwiic_OLED_1.5-Shapes.gif "Click to enlarge")
</figure>

## Example 06 - Clock

The sixth example draws a clock face on the OLED that updates roughly every second to keep time. Open the example by navigating to **File** > **Examples** > **SparkFun Qwiic OLED Arduino Library** > **Example-06_Clock**. Adjust the OLED defines to select the 1.5" display and if you want to have it keep accurate time, you can set the initial time by adjusting the initial variables for hours, minutes and seconds:

``` c++
// Use these variables to set the initial time
int hours = 11;
int minutes = 50;
int seconds = 30;
```

Upload the code and when it finishes, the display will initialize with a clock face like the image below:

<figure markdown>
[![Photo showing the OLED displaying a clock face](./assets/img/Qwiic_OLED_1.5-Clock.jpg){ width="600"}](./assets/img/Qwiic_OLED_1.5-Clock.jpg "Click to enlarge")
</figure>

## Example 07 - Cube

The last example we'll cover here is Example 07 - Cube. This example creates a cube in the center of the display that rotates around its center point. Open the example by navigating to **File** > **Examples** > **SparkFun Qwiic OLED Arduino Library** > **Example-07_Cube**. 

<figure markdown>
[![Short video showing the cube demo on the Qwiic OLED 1.5](./assets/img/Qwiic_OLED_1.5-Cube.gif){ width="600"}](./assets/img/Qwiic_OLED_1.5-Cube.gif "Click to enlarge")
</figure>

This example has plenty of variables we can adjust to change things like the size, location and rotation speed of the cube. For the video above, we doubled the size of the cube to make it easier to see. Try playing around with the different variables and re-uploading it to change the appearance and movement of the cube.