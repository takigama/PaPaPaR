# PaPaPaR

Short for Paste and Pick and Place and Reflow.

This project is an attempt to create a board that will do solder paste,
pick and place and lastly reflow. Initially I'll be aiming souly at the
pick and place stuff but theres enough componentry on the board to
control the paste and reflow components as well.

It does have enough componentry to also do a single extruder 3d printer
which wasnt exactly a goal, but was a handy alternative function for
the board. 

The board itself is reasonably compact but not a huge amount of work
has gone into it yet.

## Usage

Well, none yet. Haven't even printed the board yet. Currently using
RAMPS as a test bed.

This project is based on the STM32F103 chip and will (at least
initially) use the STM32duino code base with the arduino software
stack for making the thing "go"

You'll need kicad if you want to see the board and once i have a
working model, i'll share it as a project on oshpark!

## Thanks

Thanks go to the folk who do arduino, the folk who do stm32duino, to
the folk who do KiCad and many others probably. As of the current version
the only hardware designer is me... Im also the only coder... and the only
everything else but would welcome others

## Where it starts

The first version will be quite simple. Designed to be controlled with
2 "wiichucks", there is an expectation of having a camera and the pick
and place will be done "manually" but all electrically - i.e. you'll
place componets using joystick with some interesting hot keys and a bit
of camera work.

## It Looks Like This:
![Top](https://rawgit.com/takigama/PaPaPaR/master/hardware/pandp_s.png)

## What you need

- 3 Steppers (one for the pump)
- Perastaltic pump that can be driving by stepper (or 5-6v DC)
- a pick-up sucktion cup (i have a design for this thats really simple)
- a usb microscope.
- a design for it all to sit on
- a fair amount of imagination and pixie dust!

The pump (which is used to hold components) can either be stepper driven
or you can find plenty of 5-6v aquarium pumps on ebay that should surfice
but they want to be less than 1A.

Currently im working on the design of the actual platform for the whole
unit and it will look like a distant cousin of something like the mendel
90 (my fave 3d print) but with a stationary platform and a cartesian type
head. I was VERY tempted to do a delta but am shelving that idea for now

Currently there also exists no code but watch this space - some will
definitely be borrowed from the sprinter/marlin code bases but no code
yet exists.

