Total Hours: 6

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


