# TI-84 KE
In this repo are the files and instructions associated with the TI-84 KE as discussed here:

https://www.cemetech.net/forum/viewtopic.php?p=289588


## Parts Included:
* PCB
* 52x Keycaps
* Stainless Steel Plate
* 3D Printed Case
* 3D Printed Bezel
* 10x M3 Bolts
* 2x Ribbon Cable Extenders
* Ribbon Cable Wire
* 4x Rubber Feet

## You Will Need:
* Sacrificial TI-84 CE (Instructions written based on Rev.N, non-Python)
* 52x MX-compatible keyswitches of your choice
* Soldering Iron and Solder
* Isopropal Alcohol & Q-tips
* T5 and T6 Torx Drivers
### Optional:
* Hot Glue
* Razor/Knife
* Patience


## Assembly Instructions:

### Before assembling, please install a switch testing program onto the calculator. There are BASIC and C/ASM switch tester programs provided in this repo. You can also just make a program that prints out getKey values in BASIC.

#### Start off by disassembling you TI-84 CE:

Unscrew the battery cover and remove the battery. place the battery and battery cover to the side for future use.\
Unscrew the 6 screws around the rear poerimeter opf the calculator. Do not lose these screws. Keeps these screws for later use. On some models, there will also be screws under the battery, remove these as well.\
At this point, there should be no screw visible from the outside.\
Using an old hotel keycard or other thin plastic shim, pry the front and back halves of the calculator apart. Start from the bottom and work your way around the left (ON and Y= side), around the top of the screen, and then down towards the USB port on the right side. Angling your shim towards the front of the calculator may help.\
There will be a series of loud pops as you run your shim around the calculator. This is normal.\
Take care not to dig too deep with the shim, as you risk damaging the motherboard or screen.\
If the EMI shielding is able to be removed at this time, remove it.\
Using your fingernail or other small (not sharp) tool, release the ZIF connector that is retaining the screen's ribbon cable.\
Remove the 4 plastic rivets that are holding the motherboard in place. You can do this by putting a knifepoint or Philips head screwdriver in the middle of the rivet and twisting while applying moderate pressure.\
If the EMI shielding is still in place, it should be removable now.\
Remove the motherboard and screen from the front case. The buttons and keypad membrane will be loose in the front case, be careful not to make too big of a mess.\
Using moderate pressure from the inside, push the clear screen cover out from the front case. There is adhesive holding this cover in place, but consistent pressure should release it slowly.

#### After dissasembly, you should be left with these parts:
* Battery
* Battery Cover
* Motherboard
* Screen
* Screen Cover
* 6x T6 screws

#### Next, Assemble the switch/PCB/plate stack:

Unscrew the steel plate from the base. Use a T5 driver to remove the 10 M3 bolts. Do not loose these bolts. Inside you will find the PCB.\
If the switches you chose support LEDs from the bottom, and you want LEDs, solder the LEDs onto the PCB now, making sure of the orientation (long leg of the LED goes to the '+' sign on the PCB).\
Take 6 of your keyswitches and snap them into the steel plate at the locations pictured below (At all the "corner" locations). The pins on the bottom of the switches should be facing towards the bottom (long) edge of the plate.\
(INSERT IMAGE HERE)\
Line the PCB up with the switch pins. If your switches are PCB-mount (5-pin), press the switches into the PCB until they sit flush. This may take more force than you expect. The pins of the switches should line up with the soplderable holes on the PCB.\
With the plate/PCB/switch assemble laying face-down, ensure that the PCB is pushed or laying flush against the bottom of the switches. If you have LEDs installed, make sure they are aligned correctly.\
Solder these first 6 switches into place.\
Turning the PCB bakc face-up, insert the rest of the switches into place. Ensure that the pins on the switches are straight before attempting to put them in. There will be a distinct snap when the switch locks into the plate. If you have 5-pin switches, you may need to apply pressure from the PCB and squeeze the switch into place. Ensure that the switch bottoms are flush with the PCB, and that no switch sticks up highter than others.\
Solder the rest of the switches in place. There are 2 solderpoints per switch. If you notice one of the switch pins got bent while inserting, you can remove the switch before soldering, straighten the pins, and insert again.\
If your switches support LEDs from the top, and you want LEDs, push the LED legs through the switches and solder them now. Ensure they are and flush and "pushed down" as possible while soldering, as to avoid them interefering with the keycaps.

#### After this, you should have a complete plate/PCB/switch assembly, with LEDs optionally installed.

#### Now we will combine the base, PCB, and motherboard:

With the motherboard component-side-up, solder the reset switch wires from the base to the motherboard.\
Insert the ribbon cable extension into the ZIF connector on the motherboard.\
If you are usign LEDs, solder wires from the battery testpoint to the PCB, and 5 wires from the PCB to the blue daughterboard that is located in the base, as pictured below:\
(INSERT DAUGHTERBOARD WIRING HERE)\
Flipping the motherboard so the keypad contacts are facing up, line the USB port with the hole in the back of the case. The reset switch wires should fold and tuck under the motherboard without crossing into the battery area.\
Use 4 of the T6 screws from the calculator's case to screw the motherboard into the plastic standoffs in the bottom of the base.\
At this point, the motherboard should be screwed onto the base (keypad-side-up), the USB port should be lined up with the hole in the case, the screen extension cable should be connectd to the motherboard and laying across the base, and the reset switch wires should be soldered top the bottom of the motherboard.\
Lay the switchplate facedown at the bottom of the base, oriented as if you took the top off the base and "unfolded" the switchplate from the top.
Solder wires from the PCB at points labebled A-H to the motherboard as pictured below, according to the wiring diagram below.
Solder wires from the points labeled 1-7 to the motherboard as pictured below as well.\
(INSERT WIRING PICTURES HERE)

#### At this point, the keyboard should be functioning. Let's test it now:

Lift the base and slot the battery into place from the bottom, ensuring it is making good electrical contact.\
Gingerly connect the screen to the end of the ribbon cable extension\
If you are using LEDs, press the 4th switch from the left onm the bottom row. This should toggle the LEDs on and off.\
Press the switch 3rd from the left on the bottom row. This should turn the calculator on.\
If your calculator turns on but is unresponsive, then there probably is a short across a keypad contact, caused a key to be "pressed" constantly. Check all pads on the motherboard and switches/wires on the PCB for shorts.\
Launch your switch tester program and make sure that all of the switches work and are recognized by the calculator.\
If certain groups of switches are not responsive, check the wiring and soldering of the wires going from the PCB to the motherboard. There cold be a disconnect or a short.\
Test the reset buttom to make sure the calculator resets its ram.

#### Once all the switches work as intended, turn off the calculator and remove the battery, and unplug the screen from the ribbon cable extender.

#### Final Assembly:

While folding all of the wiring neatly, lay the switchplate assembly on top of the base. The steel plate should lay flush against the top of the base without needing to apply too much pressure. Rearrange the wiring until that happens.\
Secure the swtichplate to the base by screwing in the 10 M3 bolts. To not overtighten, as you risk stripping the plastic that the base is made of. If you do strip the plastic, you can purchase M3 threaded inserts, drill the hole a little larger, and melt the inserts into place in the base.\
Fish the ribbon cable extension out form the case through the opening for the screen. Connect the screen to the ribbon cable extendor's ZIF connector.
Place the screen into the back of the 3D printed screen bezel. Using the plastic pieces provided, clip the screen into place. You may want to secure the plastic clips with a bit of hotglue. See this picture for reference:\
(INSERT SCREEN BEZEL ASSEMBLY PICTURE)\
Being careful with the way that the ribbon cable folds/lays, snapo the screen bezel into the steel place. Start by slotting the bezel into the top edge of the hole, then pressing down firmly around the edges. The flange around the bezel should sit flush with the steel plate.\
Turning the KE over, insert the battery and put into place the battery cover. It should be a tight fit for the battery cover. Using a medium pressure, screw the battery cover into the back of the base, making sure to not overtighten or strip the plastic.\
If desired, adhere the rubber feet into the 4 corners on the bottom.

## Now, flip it over, turn it on, and enjoy your TI-84 KE1
