# TE-1-5-LIGHT-THE-LED

https://easyeda.com/editor#id=3e553166374144af88f248e61abce827|df0667116f9141a284b915eca166ce92

![](https://github.com/SteveJustin1963/TE-1-5-LIGHT-THE-LED/blob/master/LTL-cct-1.png)

## COMPONENTS YOU WILL NEED:
* R1 resistor 22k 1/4watt 5%
* R2 resistor 2k2 1/4watt 5%
* R3 resistor 2k2 1/4watt 5%
* R4 resistor 1 kO 1/4watt 5%
* C1 electrolytic 2.2 mfd 10v
* C2 electrolytic 4.7 mfd 10v
* D1 —D6 1N 914 or 1N 4148
* LED1 Light Emitting Diode
* IC1 counter IC CD 4017
* .01" thick springy brass strip
* Battery Clip
* 9v Battery
* "Light the LED" PC Board 

A game of patience. Using just two switches, a preprogrammed combination has been set for this counting IC. I challenge anyone to break the combination within 30 minutes and repeat it! 

Here is an ideal project if you are looking for something different in electron.ics. Many times I have wished I had an electronic brain teaser to try out on a witty friend or some small present to take to a sickie in hospital. Well here it is. Most of the games available on the market are too expensive or complex while others can be unravelled in a few minutes. With this game I think I have provided an ideal challenge. I like things which look easy but prove to be difficult. The secret combination (actually it should be called permutation) is locked into the game's CD 4017 IC via the gating diodes D3 D4D5and D6so that when any of the outputs go high, the switch Sw2must be in a position so that it:earths the signal and prevents it resetting the IC via  either diode D1 or D2(which feeds the reset pin 15). The object of the game is to light the red LED. With only two switches this looks at first to be an easy matter. Why, you may think, "I'll just have to push the switches randomly a few times and eventually I must strike the right combination." Well, chances are you won't, and secondly, you will not be able to repeat your effort again if you did happen to strike it after hours of trial. I would prefer to give you no clues at all on solving the combination however you will need to test the unit and thereby I lose my strategy. Without divulging too much I'll release two small clues. 1. Connecting the battery resets the IC. 2. The first switch (called the "clocking" switch) must be pushed nine times in total and  the second switch must be pushed twice. May I suggest you try random selections for 30 minutes to satisfy yourself that even with two major facts known, the combination is'still securely locked into the puzzle. After tiring of this, settle down and compile a table showing ail the possible combinations. Using this table will remove repetitive operations and you will most probably light the LED

## HOW DOES IT WORK?

![](https://github.com/SteveJustin1963/TE-1-5-LIGHT-THE-LED/blob/master/hwitwrks.png)

Fig. 1 gives you no idea of the operation of the circuit. I have drawn it this way for two reasons. Firstly, it makes the circuit very simple (which it is) and secondly, if someone asks you to see the circuit to try and work out the combination, he will be completely lost. Connecting the battery will reset the counter so that output pin 3 will have a high voltage on it. Pressing the "clock" switch Sw1 will make pin 3 go low and pin 2 high. The high will pass through D4 and into the 2k2 load R2 if switch Sw2is in the up position. If Sw2is pressed at any time pin 2 is in a high state, the voltage will pass through D2 and reset the counter back to pin 3. There are four such hidden reset paths which have to be correctly manipulated for the signal to make 9 jumps and finally light up the red LED. This may look simple but believe me, if someone handed you the finished project and asked you to decipher the combination you would be at a loss completely. I have another project at a later date in which the timing is absolutely critical and yet another which has high cycling on each switch, so an outsider doesn't know which variables are important and it is left for him to show his ability. The main reason we draw the IC as a vacant block (apart from simplifying the schematic) is due to the manufacturer rarely releasing the circuitry. Of those schematics which have been released the circuitry is so complex that it would fill up an entire page of this magazine. The internal workings of an IC is of little importance to us. We are mainly concerned with the function of each pin and the overall capability of the little 14 pin wonder. We can let you into a little more detail, however, and reproduce all the IC pins to show how the 10 outputs are turned on and off one at a time, each time the input pin is "clocked". Clocking means applying a pulse to the input pin 14.  The output pins turn on and off sequentially according to this pin order: 3-2-4-10-1-5-6-9-11. This can be quite confusing as it is not in order of the pin numbering on the IC! This unfortunate sequence has come about in the designing process and it sometimes makes printed circuit construction very difficult. For this project I have used some of the printed circuit as a platform for the switches. Utilizing the copper as a base makes the switch rigid and integral with the board and saves about $1. By using the PC board upside down the IC and  the parts can be mounted on top of the solder-lands quite easily. There is no need to drill any holes and this is an additional saving. The third and most important reason for using an undrilled board is the ease of removing the parts once the project is no longer required. I hope this will never be the case! Should you wish to "borrow" the IC at a latter date for another project all you need do is sit the board upright, hold the ends of the IC with your fingers and run the soldering iron down a row of pins. This will make the IC come partly off the board and by running the iron down the other pins the IC will come away cleanly. What a contrast to removing an IC from a normal PC board. Usually it's an almost impossible task without a solder sucker or desoldering iron and plenty of patience. 

## MOUNTING THE PARTS
![](https://github.com/SteveJustin1963/TE-1-5-LIGHT-THE-LED/blob/master/pcb1.png) ![](https://github.com/SteveJustin1963/TE-1-5-LIGHT-THE-LED/blob/master/pcb2.png)

The two switches are fabricated. This means you will be making the switches yourself from two pieces of springy brass and two saddles cut from resistor wires. Cut two pieces of brass 2.5cm long x .7cm wide (1" x 1/4") from .010" brass sheet. Tin one end of each strip and solder it onto the large copper land on the printed circuit board. Make sure they are parallel to each other and come right down to the bottom edge of the board. Curve them upwards so they have a 1cm travel to the PC board. Make two staple-looking saddles from wire cut off a resistor and trim the legs short so that when you place them over the brass strips they press fairly hard on the brass. Solder them in position making sure the strips still have some travel left to touch the printed circuit contacts below. Dimple the centre of each saddle to make a point contact. Mount all the other components .as shown in the layout diagram except the two top diodes D1 and D2. These will be soldered in after the unit has its pre-test. The other diodes and resistors can be left standing up from the board to reduce congestion. Hold each part in your fingers as you solder it. If you find the parts getting too hot, you are taking too long to solder them. This is the easiest way to judge if you are good at soldering. Here are three tips to speed up your soldering: 1. Tin each lead of the component first. This is a must. I always do this before soldering any parts into a project. 2. Use only a fine tip soldering iron. Preferably use a constant temperature soldering iron for fine work like this. 3. Use FINE solder. Old fashioned 16 and 18 gauge solder is OUT. 

## TESTING THE UNIT
All the parts should be soldered in place as shown in the diagram except the two top diodes D1 and D2. Connect only their cathodes (marked with a band) to pin 15. Connect the other end of Di via a jumper lead to the negative lead of the battery. The reset pin must not be left open or floating as this will prevent the IC from clocking. Connect a 9v battery to the battery clip. Push Swi ten times and the LED will light up. Try this a number of times. You are cycling the Decade Counter. Notice you must push the switch slowly and firmly as any contact bounce will register on the IC very easily and the LED will light up after pushing the switch only 6, 7 or 8 times. A considerable amount of contact bounce has been eliminated by the inclusion of the 2.2mfd and 4.7mfd electrolytics. Without them the bounce from five pushes will register as a count of ten. Disconnect the battery and solder D1 into circuit Connect the battery and cycle the counter via Sw1 The LED should not light up even after 50 pushes. If it does light up, Sw2 is not making connection at its upper contact. Press Sw2 down any cycle the IC. After each ten clocks the LED should light up. Disconnect the battery and solder D2 onto the board. Make sure Sw2 lower contact is working by soldering a bump of solder onto each surface and cleaning with a small file. Now try to light the LED! 
