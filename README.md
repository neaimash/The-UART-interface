# The-UART-and-SPI-interface
Two programs, which are designed to run a step in which two development circuits are connected to each other.
One development circuit (the master) communicates with the computer via the UART interface, and the other (the slave) communicates with the master
Also, the slave is connected to a motion sensor via the SPI interface.
The programs do the following:
1. When the master starts working, he prints to the computer he is working on.
2. When the slave starts working, it prints to the computer it is working on.
3. The LED on the development circuit of the master flashes at a rate of half a hertz. (That means it will turn on for one second and it will be
Off for one second, and on again, God forbid.)
4. The LED on the slave's development circuit flashes at a rate of 1 Hz. (That means it will turn on for half a second and be off for half
a second, and God forbid.)
5. The slave's software maintains a clock that works with a resolution of seconds.
6. There is an option to give a command from the computer to the master, following which the current time will be determined on the slave, in the format
of hours, minutes, and seconds.
7. When the motion sensor detects motion, the master prints to the computer a message that motion was detected, and the time
The current one (which is read from the slave) in the format of hours, minutes, and seconds.
