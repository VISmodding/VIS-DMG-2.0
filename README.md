# VIS Game Boy DMG 2.0

![image](images/boards.png)

This project was born with the aim of saving corroded boards of **Gameboy DMGs** or **SNES Super Gameboy adapter**s. For this reason, I developed replacement PCBs by using modern electronic components. Essentially this is a gameboy DMG having:
- a built-in lipo power board with charger
- analog power and button RGB LEDs
- tactile switches
- this version only support IPS screens and not the original screen with the original front PCB
- 1 watt audio speaker support
- a cool design in which the front view of the console is totally covered by the PCBs 
- mainboard and IPS board are 4-layer PCBs in which analog and digital lines are kept separated in order to minimize audio noise (separated analog/digital/power ground are kept in this version. They are connected only into a single point). Clearly audio noise cannot be completely removed since the CPU accept only an unique 5v line (without a separated analog input for the audio). Anyway, the low audio noise in this version probably is the cleaner audio you can have by using a lipo battery and the high volume provided by 1 watt speaker.

## Warning: 

<ins>Mainboard is not tested. Its prototype works after some manual fixes. These fixes then was applied to the production file. Hence, it should work but I cannot ensure it</ins>

## Disclaimer

**This is a DIY project for electronic enthusiasts. For this reason, I am not responsible for any damage incurred while attempting this project or after completion of the project. You alone accept all risk since you are 100% liable for damage to yourself or your property.**

## Boards compatibility

  - Audio board is not compatible with exisisting gameboy boards. Since in this version audio amplifier is on the mainboard the audio board is not compatible also with my previous gameboy.
  - Other IPS boards can be used with this realese but the following jumpers must be left open. In any case the speaker must be always connected to the audio PCB and not on the IPS PCB.

![image](images/02_jumpers.png)

## Instructions

Start by soldering firstly the U3 boost Ic and check solder continuity/no bridges by using the zoom in the following image. Then, populate all the power board and test the 3.3v and 5v lines (see the image) and also test the charging circuit as explained in the [setup video DMG v1](https://youtu.be/e4qCekoWYW4) of previous DMG version. Note that, for the charger, you can use in this version the SMD LEDs (green and red) or the 3mm LEDs (they are usefull if you don't use a tranpsarent shell. Hence you can make 2 holes and put properly the LEDs in order to see lights when charging).

![image](images/01_PB_popul.png)

When you are sure on the power board installation you can proceed to populate all the boards. See in this case also the [setup video DMG v1](https://youtu.be/e4qCekoWYW4) to understand how solder the IPS wheele and the audio taller.

I remember you that all the tactile switches must be soldered with the orientation shown in the following old image 

![image](images/buttons_orientation.jpg)

**To be continued

**WARNING** Don't do a bath of 15/30 minutes for the IPS board if tactiles are installed (keep them outside the IPA; otherwise, the glue that keep metal pieces will be dissolved and switches break). I solder the tactiles after the bath in IPA without using additional flux (I simply exploit the flux of the soldering tin).

**SUGGESTED ITEMS**: I suggest using a 5v 2A USB-C charger with the 2A cable USB adapter (I suggest the right angle version) that can be purchased here [Link Aliexpress](https://www.aliexpress.us/item/2255800098767754.html?spm=a2g0o.order_list.order_list_main.35.f4763696ab50XM&gatewayAdapt=ita2usa4itemAdapt)

Finally, I suggest to use full silicone buttons from Kitsch-Bent as shown in this [short video](https://www.youtube.com/watch?v=DBGJTIemyE4&t=64s&ab_channel=V1sModding).

**NOTE**: When you start to hear aliens coming from the speaker and the screen starts flashing, it means that you have to charge the battery. I have not disabled the CPU in this case to give you the time to attach the power supply without losing the game in progress!!!

## Credits

  - [Bucket Mouse](https://github.com/MouseBiteLabs/) for the [DMGC](https://github.com/MouseBiteLabs/Game-Boy-DMG-Color) project from which I get the RGB LEDs idea, the correct position of some holes, the audio amplifier location and the tactile buttons model

  - [consolesandcasks or Deceptive thinker](https://github.com/consolesandcasks) for another [Heavy CPU MGB](https://github.com/ConsolesandCasks/CPU-MGB-Heavy) project that I referenced and utilized to update the actual DC Jack

  - [Kamicane](https://github.com/kamicane/) for the [Super DMG](https://github.com/kamicane/Super-DMG-01) project from wich I get the audio board shape

  - [Gekkio](https://github.com/Gekkio/) for the [DMG](https://github.com/Gekkio/gb-schematics/tree/main/DMG-CPU-06) schematics

## FAQs

link [here](FAQs.md).

## Troubleshooting

link [here](troubleshooting.md).

## Acknowledgements

I would like to thank Mathijs (the creator of SYF Game Gear PCBs) for his several suggestions, schematics, and help in this project. I would like to thank also Luke from Retrosix for some usefull suggestions.

## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>. You are able to copy and redistribute the material in any medium or format, as well as remix, transform, or build upon the material for any purpose (even commercial) - but you **must** give appropriate credit, provide a link to the license, and indicate if any changes were made.

## Support VIS projects

I have several stuffs in mind, but since developing these things has a high cost in materials and prototypes, a little [PayPal](https://www.paypal.com/donate/?hosted_button_id=64CARRQYFEZYL) donation is appreciated.

## Contacts

**email**: vis.modding@gmail.com <br />

**discord**: you can find me as *vis_modding* on several servers (BennVenn, Mouse Bit Lab, Retrosix modding, Game Boy, Gameboy makers).
