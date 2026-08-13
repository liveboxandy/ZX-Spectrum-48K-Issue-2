This is a Kicad 10 project for an issue 2 16/48K ZX spectrum.

It was only done in order to produce an interactive bom (ibom.html) to aid in the debugging of faulty Speccies.
Although the gerbers appear to be correct to the original PCB I would not use them to get a PCB manufactured without a lot more checking.

It was created by overlaying pictures of a raw Issue 2 PCB, topside and bottomside in Kicad's PCBNew program and then creating the pcb layout from those and a readily available schematic. 


Where there are differences the pictures took priority for routing and connections.

Where possible the Sinclair routing has been followed, including all the ground planes. 


Various mods have been released and the following have been applied to the pcb and schematic layout,

D14 replaced by C67 (100pF)                                         - Machine Code fix

R24 changed from 3K3 to (1K)                                        - Machine Code fix

R27 changed from 680R to (470R)                                     - Machine Code fix

R73 added between IC1/32 and +5V (1K)				    - Machine Code fix

C51 in layout between NMI and GND is not fitted, value unknown      - Not fitted

R60 changed from 100R to (270R)                                     - PSU Fix

R48 changed from 4K7 to (2K2)                                       - Colour quality

R49 changed from 18K to (8K2)                                       - Colour quality

R50 changed from 8K2 to (4K7)                                       - Colour Quality

R72 changed from 18K/47K to (10K)                                   - Colour quality

C65 changed from 100uF to (22uF) and positive identified correctly. - Colour quality

The following components do not have positions on the PCB and have to be fitted across other components,

TR6 ZTX313 added to schematic, but not in PCB layout. Base-IC2/30(A0), Collector-IC2/11(+5V), Emitter-IC1/33(IOREQ)

C74 47uF added to schematic but not in PCB layout. +ve TR5E/C34+, -ve TR5B(R58Left) - PSU Fix

ULA 5C112 requires the following,

R47 220R

R49 8K2

R56 220R

R63 220R


ULA 6C001 requires the following

R47 1K

R49 10K

R56 470R

R63 470R

According to the Service Guides, IC25/26 74LS157 should NOT be of NatSemi make.

