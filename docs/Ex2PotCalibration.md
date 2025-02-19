# Calibrate Potentiometer Angle

## introduction
<debugHL> Aim</debugHL>

!!! Info "GTA Marking"
    This is an assessed Exercise. When you have completed exercise, you should show your work to a GTA to get marked.

!!! Note "Before Continuing"
    Before starting these exercises, you should ensure that you have completed the LED Pattern exercise and have the potentiometer and LED still connected. You should also read the <debugHL>[Analogue Sensors](./Background.md#analogue-sensors)</debugHL> section of the Background page. 
    

<problemHL>Can We get a Tinker CAD Drawing of the LED, Potentiometer and Button Circuit on Breadboards</problemHL>

A quick video demonstrating the final system is shown below:

<div style="text-align: center;">
<iframe id="kaltura_player" src='https://cdnapisec.kaltura.com/p/2103181/embedPlaykitJs/uiconf_id/53345422?iframeembed=true&amp;entry_id=1_a3eviyhm&amp;config%5Bprovider%5D=%7B%22widgetId%22%3A%221_4q6vxp1v%22%7D&amp;config%5Bplayback%5D=%7B%22startTime%22%3A0%7D'  style="width: 400px;height: 285px;border: 0;justify-content:center;" allowfullscreen webkitallowfullscreen mozAllowFullScreen allow="autoplay *; fullscreen *; encrypted-media *" sandbox="allow-downloads allow-forms allow-same-origin allow-scripts allow-top-navigation allow-pointer-lock allow-popups allow-modals allow-orientation-lock allow-popups-to-escape-sandbox allow-presentation allow-top-navigation-by-user-activation" title="Placeholder - Quick Test Video"></iframe>
</div>

## Exercise

The map function can be used to provide a linear calibration between a measured value and a real world parameter. In the case of the potentiometer test circuit, the potentiometer has a rotational range of 300°. 

The aim of this exercise is to use the map command to produce a calibrated potentiometer angle, using the ADC measurement as an input, and write the potentiometer angle to the serial monitor.

**Procedure:**
 
1.	<debugHL>The starting point for this exercise is the Potentiometer test circuit, you have constructed, and the Potentiometer test program from the previous exercise.</debugHL>
2.	Add a map() function to the sketch to calibrate the potentiometer angle between -150 and 150 for an ADC measurement input of 0 to 1023.
3.	Using the Serial.print() and Serial.println() functions, (similar to that shown in <debugHL>POT.ino</debugHL>), write the data to the serial monitor with appropriate description.

!!! Info "Serial Communication Functions"
    See the serial communications functions page from the Arduino language reference pages for a description of the Serial.print() and Serial.println() functions: [https://www.arduino.cc/reference/en/language/functions/communication/serial/](https://www.arduino.cc/reference/en/language/functions/communication/serial/ "Link to the Arduino reference pages for the serial communications library")

**When completed, your code should function as follows:**

* When you rotate the potentiometer, the serial monitor should display the ADC read value and the potentiometer angle, in degrees.
* The serial monitor should update at a reasonable rate – 2 to 4 times a second.

!!! Success "Now Get Your Work Marked by a GTA"
    Once you have completed your code and are satisfied with its operation, you should show your work to a GTA for marking.