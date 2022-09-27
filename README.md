# DIY Forth Interpreter
In the early 80's I bought a Noth Star Computers Horizon S100 computer. The OS was CP/M. I used it to put together a two axis data collection, correction,
and validation system for our CalComp digitizers. For the application code I started with the article "Write Your Own FORTH Interpreter", by Richard Fritzson,
in Kilobaud Microcomputing, February 1981 page 76 - 92. I typed in and compiled the Forth interpreter as the foundation of the control software that I wrote.
The article can be found in the public domain in the Internet Archive at:
https://archive.org/details/kilobaudmagazine-1981-02/page/n75/mode/1up?view=theater
 
I am "copying" all of the listings, minus the hexidecimal bytes, for re-use here. My plan is to later branch this to an #RC2014 robot project.

To copy the listings I used the Archive to export a PDF of the magazine. I cut and paste the listing code into forth.asm, created with 
Notepad++ (https://notepad-plus-plus.org/). This is not quite as easy as it sounds, but it seems easier then retyping it all.
As I said, my goal is to run this on a #RC2014 Z80 computer, but to compile and test it, it is faster to use the CP/M emulator
MyZ80 (http://z80.eu/myz80cpm.html) running under DOSBox (https://www.dosbox.com/). I am including my DOSBox configuration file in this repository. 
It simply sets cycles=max, mounts a DOS C: drive, and starts MyZ80. Depending upon your system, you can just leave it running minimized until needed.
From the CP/M command line I switch to the C0: drive and import forth.asm. To compile it I simply type "asm forth". This lists any  errors and
generates, amoung others, a forth.prn file. I export the .prn file and keep it open in Notepad++ for update and review.
