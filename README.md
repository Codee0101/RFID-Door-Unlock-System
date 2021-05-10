# RFID-Door-Unlock-System

This a software simulation of RFID based Door Unlock System on Proteus.<br/>

## Installing Proteus

You may install the licensed version of proteus(paid) or can also get latest unlicensed [version](https://getintopc.com/?s=proteus) (not recommended but you can go with it if that is the only option left).
After installation, if the components list shows as empty, follow this [link](https://youtu.be/l4770kWKwRs).<br/>
Once the installation has completed, you can open the Project file (with extention .pdsprj) and modify it according to need.

## Installing Keil uVision

You can skip this step if you don't wish to change the code. <br/>
Download the Keil MDK-Arm and Keil c51 (both are free) from the [official Keil website](https://www.keil.com/download/product/). It would ask for a bunch of information before you can start installation.

## Debugging the code in Keil uVision

You can skip this step if you didn't change the code. <br/>
1. Create a project (.uvproj)
2. Import the code from the location where you have downloaded this repository.
3. Right click on the Target 1. 1. Go to the 'Target' tab and check that the crystal frequency matches to that of the one set in the microcontroller in Proteus. Next, go to the 'Output' tab and select 'Create HEX File' check-box and hit 'OK'. 
4. Here, you can edit the code according to your need (changing the delay time, message to be displayed, etc).
5. Now, Translate and Build the file in Keil. You will notice that a new HEX file has been generated.

## Loading the code in Proteus

You can skip this step if you didn't edit the code. <br/>
1. Right-click on the microcontroller in Proteus and select 'Edit Properties'.
2. In the 'Program File', make sure that the correct HEX file (the one you recently generated) has been selected.
3. Click 'OK'.

## Running the Simulation

1. Select the 'PLAY' button on the bottom-left corner. A 'Virtual Terminal' pop-up would open on the screen. <br/>
2. Enter one of the 3 correct IDs from the code(you can also insert your own, just make sure they are 12-digit long). <br/>

The LCD will display the authorisation message (which you can edit in the code) and the motor would start rotating to unlock the door(visual representation).<br/>
If any other input is given, the LCD will display the rejection message and the door will continue to remain in locked state.

<br/>
