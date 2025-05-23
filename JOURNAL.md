Total Hours: 12

##  Initial layout (2 hours)

I have researched Apple and apple clone keyboards. 

![image.png](/PCB/Images/image.png)

I will be baseing my keyboard off of this design with a few added features.

New features:

- USB-C power
- Mechanical switches
- Rotary encoders
- volume fader

I started by mapping my keyboard matrix. I am using MX alps hybrid footprints to give a wider range of options for switches.

![image.png](/PCB/Images/image-1.png)

This layout closely mimics the original layout with few changes. Having that finished, I have begun to research QMK compatible controllers for the next step.

##  Microcontroller (2 hours)

I am using an AT90USB1286 controller (due to its USB functionality and QMK compatibility). The controller is connected to a 16mhz crystal for timing. The CC pins on the USB-C port are pulled down to ground via 5.1k resistors to follow the USB-C specification. I have 2 rotary encoders (EC11) and the special feature of my project, a fader for volume control. Capacitors 1 to 7 are used for decoupling and filtering.

![image.png](/PCB/Images/image-2.png)

The columns from the layout have been connected here to the matrix above. I have also conencted up the two rotary encoders and the slider fader. 

##  Layout (2 hours)

![image.png](/PCB/Images/image-3.png)

Next i laid out the keyboard in the most optimal format for the space. This format allows me to make versions with and without the fader + rotary encoders. I also rounded the PCB edges and added 3.2mm screw holes for mounting inside a case. I have ensured the pcb is less than 50cm long to ensure it can be assembled with many assembly services.

## Back to the drawing board (2 hours)

![image.png](/PCB/Images/image-6.png)

Due to using a non standard layout, I found it would be impossible to get keycaps for some keys (such as my thin iso key). I am instead using a more standard layout. Because of the saved money from doing this, I can now add LEDs. I have added a backlight led matrix that can be controlled via the MCU. I have created my new layout, connected it to the MCU schematic and added LEDS with a driver.

![image.png](/PCB/Images/image-5.png)

## New Layout (2 hours)

I laid out the PCB again with the new logic for the LEDs.

![image.png](/PCB/Images/image-4.png)

I have added a resistor to 5v for each led and laid the pcb out similar to before.

## Routing (2 hours)

I routed the PCB and added a ground plane.

![image.png](/PCB/Images/image-7.png)

![image.png](/PCB/Images/image-8.png)

Although my ground plane is missing from a large part of the PCB, it still links all ground traces together well. I also added 4x m3 screw holes for mounting.