This git repo is a submodul of an fpga based project.
Implements a high-resolution pwm with axi (xilinx) bus slave interface.

Registers (offset*4 byte, description)
0: control and status
1: cycle time 
2..4 start compare reg
5..7 stop compare reg

Output bus type is xilinx:GPIO for 3 pins.
(tristate ports are at always zero level and input ports are implemented but not used by design.)
Tested and developed with Digilent CmodA7-35T board.