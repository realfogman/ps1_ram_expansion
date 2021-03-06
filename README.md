# IBM PS/1 (model 2121) 4MB Memory Expansion
This is a 4MB memory expansion card for the IBM PS/1 model 2121 with a Intel 80386 CPU.
The schematic was done in Kicad (https://www.kicad.org/).

![Top view](ps1_pictures/board_top_scaled.jpg?raw=true "Top view of the finished board")
![Bottom view](ps1_pictures/board_bottom_scaled.jpg?raw=true "Bottom view of the finished board")

The memory expansion board was tested with CheckIt 3.0.
The memory ICs (2x IC41C16100S-50KG) can be found on different platforms and are still cheaply available.

# Disclaimer and attention
Although the board works for me in my setup, don't make me responsible if it does not work for you, or (in the worst case scenario) if it breaks your PC.
This is a hobbyist project with no guarantee of functionality!

Please don't forget to close the solder jumpers according to the top view.
Otherwise, the IBM PS/1 won't or wrongly detects the inserted RAM size.

In order to fit the board into the memory extension slot, don't forget to cut the connector board between D13 and D14 (according to the image).
Please, watch out to not cut any traces!


# Issues and improvements
My first attempt was quick and dirty (missing drilling file and mirrored text on the pcb bottom side) ;(

Luckily JLCPCB (https://jlcpcb.com/) checked my design and we could resolve these issues.

The Memory ICs have multiple VCC pins, which should be decoupled with 100nF capacitors each.
These capacitors could be located on the bottom side of the PCB board.
In the initial project release, only one 100nF capacitor is used.
