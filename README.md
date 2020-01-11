# MHW_CTC_Template
Binary Template for the 010 Editor that allows for jigglebone physics editing in Monster Hunter: World

_This template was created by Karbon, my limitless thanks goes to them!_

***
This file requires the 010 Editor found here: https://www.sweetscape.com/010editor/

To use it, follow these steps:
1. Open up the 010 Editor, go to the upper toolbar, and pick "Templates > View Installed Templates"
2. Press the Add button and locate the "CTC_Template.bt".
3. Once added, hit OK to return to the software.
4. Now that the template is saved, any time you open a .ctc file of your choosing and press F5, you can select the CTC_Template option. 
6. The hex window should now be colored and a result window pops up to allow modification.

Have fun!

***
ICEBORNE UPDATE:
- Template now reads updated bones properly (they added a 16 byte line to the end of all bones)
- Color coded important parts of bones.
- Added section on bones for their collision radius.

TO FIX YOUR OLD CTC FOR ICEBORNE:
1) Open your .ctc with old template
2) Change the 5th byte from 1B to 1C
3) Add this line of hex to the end of EVERY bone (every 7th line down, insert with Ctrl+Shift+V), DONT OVERWRITE

00 00 80 3F CD CD CD CD CD CD CD CD CD CD CD CD

Save and load the new template to check.

![Example image of new bones](https://cdn.discordapp.com/attachments/481188093123231764/665446423877255182/unknown.png)

_Thank you to Ice for finding the new hex!_

Something Ice wanted to point out:
> Most of the time the end child bone has 00 00 80 3F (1.0)

> However for the rest of the child bone they usually have 00 00 00 80 (-0.0), though this value varies with in 0-1?

Putting that hex into every bone seems to be fine, but it might be good practice to replicate what iceborne .ctcs do.
