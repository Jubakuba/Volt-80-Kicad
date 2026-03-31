# Percent Stuidio VOLT 80 Replacement PCB Project

This PCB can be purchased and assembled by JLCPCB or other services.  You can have them assemble hotswap socket of your choice or order them and solder them yourself.  I'd recommend top assembly option at minimum for the PCBA (see LED and capacitor spacing).

## Documentation

* [QMK files (I'm going to make it officially merged hopefully)](https://github.com/Jubakuba/qmk_firmware/tree/master/keyboards/percent_studio_aftermarket)

* This PCB does not have per-key RGB or battery support as the original one does.  It adds custom firmware support and flashing without a .zip file passed around 200x online instead.  4 LEDs can be configured via software at the original LED window on the keyboard.

* If you would like to modify the PCB - the Library files may need to be modified.  In Kicad:  Preference: Manage Footprint Libraries.  Ensure the Library within this Github is added.

## Build Instructions

[qmk.fm](https://qmk.fm) is the official website of QMK, where you can find links to this page, the documentation, and the keyboards supported by QMK.

Pull [my fork](https://github.com/Jubakuba/qmk_firmware/) in the event you don't see "percent_studio_aftermarket" as an official keyboard.

Buy a [Waveshare RP2040-Tiny](https://www.waveshare.com/wiki/RP2040-Tiny) to control the board.  Amazon often has them as does the official Waveshare site.

Sand off the corner edges of the purchased controller:
![USB Daughterboard](https://i.imgur.com/CS0CqIU.png)

This will allow the controller to mount into the frame.
![Mount](https://i.imgur.com/59MqcoC.png)

You may either have to sand some height off of the board mounting screws or put a shim under the board for it to press hard on the board.  This isn't necessary for it to hold it in place and allow use.  But it will wiggle as you insert the USB.

Order the PCB.  The default .zip file will allow JLC to assemble both sides by default.  You will have to select the hotswap components you'd like (they have some) or you can consign Kailh ones.  I'd personally recommend just building it with matched components and soldering the hotswap sockets and controller yourself.

Once the PCB arrives.  Solder hotswap sockets (if applicable) and controller.  If you've never soldered: this PCB was my first project and I did it by hand with no assembly.  The switches and controller are by far the easiest pieces.  You've got this!

Keyboard done.  Connect the controller to the USB port with the included cable.  Flash the uf2 file you can compile using QMK.  Customize to your wishes.  Change layers.  Change LED colors.  Etc.