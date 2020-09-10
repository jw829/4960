---
layout: page
title: Lab 1 - The Artemis Board
---
<img src ="images/artemis.jpg" width = "200">
### Parts Needed:
* 1 x SparkFun RedBoard Artemis Nano
* 1 x USB A-to-C cable
* 1 x Li-Ion 3.7V 500mAh battery

### Video and Code Demonstration:
1. Blink it up: the following video shows the board blinking its builtin LED.

<iframe width="560" height="315" src="https://www.youtube.com/embed/njZcvr3d-II" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

2. Serial: the following video shows the working Serial port.

<iframe width="560" height="315" src="https://www.youtube.com/embed/TS8YnWNQZ3k" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

3. AnalogRead: the following video shows that the board's temperature increases after hot hair is blown onto it.  

<iframe width="560" height="315" src="https://www.youtube.com/embed/1eO07-Ztc6g" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

4. MicrophoneOutput: the following video shows that the highest frequency changes as I speak! 

<iframe width="560" height="315" src="https://www.youtube.com/embed/mEYNIKG4enQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

5. Whistling: I added a loop in the previous code file to blink the board when it hears a whistle.
```arduino
        if (ui32LoudestFrequency > 2500)
        {
            digitalWrite(LED_BUILTIN, HIGH);
            Serial.printf("WHISTLE\n");
            }
        else {
            digitalWrite(LED_BUILTIN, LOW);
            }
```
This video shows that the board blinks when a whistle is detected.
<iframe width="560" height="315" src="https://www.youtube.com/embed/KoDkX6vNTrs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


This video shows that the above still works when the board is unplugged from the computer (using battery).
<iframe width="560" height="315" src="https://www.youtube.com/embed/-92acptAEIU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>