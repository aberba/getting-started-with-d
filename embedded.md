The LLVM project recently merged an experimental AVR back-end, and as it turns out, this back-end is usable from the D programming language using the LDC compiler!

AVR is an instruction set interpreted by some Harvard architecture microcontrollers. When you compile your D program to AVR and run it on a suitable microcontroller, it will start executing the main function as usual. The program can interact with the outside world through I/O pins and interrupts.

In this series of blog posts I will be making a quartz watch with torch and radio clock synchronization. This is the first post in this series.
https://foldr.nl/running-d-on-a-microcontroller/
