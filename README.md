# kdb75-files

kdb75 configuration files

This repository contains the binary I last loaded into the keyboard, the layout I've picked and the JSON
data that can be used to load into the QMK configurator.

This is just a repository so that I can have a way of looking back at where I was months later.  Originally,
I was using the How To link below, which references a Chinese configuration tool (http://qmkeyboard.cn/).  The qmkeyboard
tool is decent, but it lacks the pre-defined configuration modes available within the QMK Configuration tool.  And that
also includes some of key codes.  That said, qmkeyboard has a way of changing the wiring (and subsequently, that will
change the layout), but the wiring diagram is far less intuitive than the simple Layouts provided by the 
QMK Configuration tool.


## Programming

Quickstart:

* Download and install QMK Toolbox
* Upload the JSON file within this repo to QMK Configuration website
* Have the QMK Configuration website build the binary (get some coffee...)
* Download the binary
* Startup QMK Toolbox app
* Put the keyboard into flash mode (fn + top-right button)
* Open the downloaded binary in the QMK Toolbox app (should point to the local file in the top text box)
* Click on Flash - wait a couple of seconds

Note: The QMK Configuration binary creates a keyboard that isn't recognized by Windows or Mac, so plugging the keyboard in may result in a popup to configure.  The popup can be safely ignored and closed.

## Layers

### Layer 0 - Windows
Key combo:  Fn + 1

This layer is a basic windows keyboard layout.  It should be immediately familiar.  I picked Layer 0 because
my family is most familiar with Windows and won't know the multiple layer layout and Layer 0 is the default
layer when plugged in.

![Image of Layer 0](layer-00.png)

### Layer 1 - MacOs
Key combo:  Fn + 2

This is the layer I'll use most often.  Each time the keyboard is plugged in to a Mac, I'll need to switch to 
this layer.

![Image of Layer 1](layer-01.png)

### Layer 2 - Gaming (Windows)
Key combo:  Fn + 3

This layer contains a standard left hand and then it's split with the right hand and the right hand has vim mouse 
controls.  While the functionality is all available for running a mouse with 5 buttons, the practical use-case for
a keyboard driven mouse is low.  A standard mouse in a gaming scenario is far quicker/more accurate especially with
camera scanning.

![Image of Layer 2](layer-02.png)

### Layer 15 - Control
Key combo:  Fn (momentary)

This layer contains control for switching to a different layer and also for controlling the lighting modes on the 
keyboard.  

Additionally, this layer contains the RESET button for flashing.  Without RESET, I'd need to unscrew the
case and access the on-board switch.  Flashing uses the QMK Toolbox.

![Image of Layer 15](layer-15.png)

## Links

### Parts
* PCB - https://kbdfans.com/products/kbdfans-75-pcb-75
* Circuit Diagram - https://cdn.shopify.com/s/files/1/1473/3902/files/Q75.pdf?9073386096780420683

### Programming
* How To - https://www.reddit.com/r/MechanicalKeyboards/comments/6hl837/kbd75_r3_qmk_howto_guide/
* QMK Configurator - https://config.qmk.fm/#/kbdfans/kbd75/rev2/LAYOUT
* QMK Keys - https://docs.qmk.fm/#/keycodes
* QMK Toolbox - https://qmk.fm/toolbox/
