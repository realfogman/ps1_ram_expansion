# PS/1 4MB Memory Expansion
Memory Expansion for the IBM PS/1 2121 80386 PC
![Top view](ps1_pictures/board_top_scaled.jpg?raw=true "Top view of the finished board")
![Bottom view](ps1_pictures/board_bottom_scaled.jpg?raw=true "Bottom view of the finished board")
The memory expansion board was tested wich CheckIt 3.0.
The memory ICs (2x IC41C16100S-50KG) can be found on different platforms and are still cheaply available.

# Attention
Please don't forget to close the solder jumpers according to the top view.
Otherise, the IBM PS/1 won't or wrongly detects the inserted RAM size.

# Issues and improvements
My first attempt was quick and dirty (missing drilling file and mirrored text on the pcb bottom side) ;(
Luckily JLCPCB (https://jlcpcb.com/) checked my design and we could resolve these issues.

The Memory ICs have multiple VCC pins, which should be decoupled with 100nF capacitors each.
These capacitors could be located on the bottom side of the PCB board.
In the initial project release, only one 100nF capacitor is used.
