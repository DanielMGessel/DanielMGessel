Hobbyist programmer enjoying Recreational Mathematics.

I'm currently working through the book “Mathematical Logic through Python” by Yannai A.
Gonczarowski and Noam Nisan (www.logicthrupython.org). In addition to the exercises in
their codebase, I'm creating my own “logic language” with some different bells and whistles.

I hope to wrap this in a Debian based “Neo-Retro” Computing Environment for exploring
Symbolic Logic and Recreational Mathematics and, with its “Old-School” nature, it should
run reasonably on current crop of Raspberry Pi computers. The open nature of the RISC-V
architecture is appealing, so I'm testing on StarFive's VisionFive2 RISC-V SBC as well. I
use an AMD laptop, running Debian's AMD64 port, for faster development while I'm dependent on a
variety of tools I'm using for bringup, and there's no reason not to continue to run on AMD64.

The portability promise of Emscripten has led me to SDL, which can run on Linux with or without
a windowing system, and the combination may be a pathway to non-Debian systems, but only if this
project actually gets to a state where people want such a port.
