#### Recreational Mathematics ∧ Symbolic Logic

I've been slowly reading [“Mathematical Logic through Python”][mltp] by Yannai A. Gonczarowski
and Noam Nisan. Following the exercises in the book, I'm also creating my own
experimental Symbolic Logic language which I call Sapphire. It's fun-and-games: exploring Sudoku
puzzles and variants as large SAT problems. Next up will be recreational problems in Number
Theory.


#### A Pi, a Keyboard, and a TV Walked Into a Bar...

I'm also working on a Debian GNU/Linux based Computing Environment, Royal, which will host
Sapphire and I'll use it to explore my interests in Recreational Mathematics further. It should
play well with the “old-school” roots of the Raspberry Pi[<sup>rigs</sup>](#rigs) and my goal is
for it to run well on a Pi Zero2 (the Pi Zero W is overburdened by my Python prototypes, but I
tend toward bit fiddling which should be faster when converted to C).


#### Debian GNU/Linux running on ARM64, AMD64 or RISC-V

While my target is the Pi running 64 bit Raspberry Pi OS Lite, my primary development machine is
an AMD-powered laptop running Debian. As a little endian 64 bit machine, I'll keep it running
there even if I upgrade my primary machine to a different architecture.

I'm also testing on StarFive's VisionFive2 RISC-V SBC; it's underpowered at a
similar price point to the RPi5 with a peak CPU clock rate of 1.5Ghz compared to the RPi5's 2.4Ghz.
The RISC-V core IP ”scene” is still immature with fewer silicon iterations to learn from - give
it time. Milk-V Mars has the same JH7110 SoC from StarFive, I may pick one up to add it to my
test farm, but it may add little. The Beagle-V Ahead may perform a little better, with a peak
clock of 2GHz and the IMG BXM GPU may outperform the IMG BXE GPU in the StarFive SoC.

SDL gives easy access to the GPU, display and input events. It can run can run
on [RPi OS][rpios] “with desktop” as well as RPi OS “Lite” (interacting with a Wayland “compositor” or
the DRI - Direct Rendering Infrascture - and reading input events via evdev).


#### Emscripten for All the Rest

Checking out the portability promise of Emscripten is what led me to SDL. For my own use,
Debian GNU/Linux is ideal, but if this project gets to a state where people would be interested
in using it, an Emscripten port might be the way to go.

##### Rigs
While the [All-in-One RPi 400][rpi400] (and presumed forthcoming RPi 500) intentionally
evokes memories of early [home] computers like the Apple II+ I grew up with, I'm imagining a
different configuration combining an [RGB keyboard][logg] and a [small touchscreen][hype]
attached to the Pi, resting below the keyboard in place of a touchpad on a laptop. All these
extras are to guide keyboard shortcuts - alternatives will work, just in case you don't want
a dedicated computer to run my code...

[mltp]:   https://www.logicthrupython.org
[home]:   https://en.wikipedia.org/wiki/Home_computer
[rpi400]: https://www.raspberrypi.com/products/raspberry-pi-400-unit/
[rpi5]:   https://www.raspberrypi.com/products/raspberry-pi-5/
[rpios]:  https://www.raspberrypi.com/software/operating-systems
[logg]:   https://www.logitechg.com/en-us/products/gaming-keyboards.html
[hype]:   https://shop.pimoroni.com/products/hyperpixel-4