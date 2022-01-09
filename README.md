# PS/1 4MB Memory Expansion
Memory Expansion for the IBM PS/1 2121 80386 PC

# Issues and improvements
The first attempt was quick and dirty (missing drilling file and mirrored text on the pcb buttom side)!
Luckily JLCPCB (https://jlcpcb.com/) checked my design and we could resolve these issues.

The Memory ICs have multiple VCC pins, which should be decoupled with 100nF capicators each.
These capacitors could be located on the buttom-side of the PCB board.
In the initial project release, only one 100nF capacitor is used.
