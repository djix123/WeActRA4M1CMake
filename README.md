# WeActRA4M1CMake
Template CMake / GCC project for R7FA4M1AB (RA4M1) found in the [WeActStudio RA4M1 Core Board](https://github.com/WeActStudio/WeActStudio.RA4M1_64Pin_CoreBoard) (and the Arduino Uno R4)

Uses [Renesas FSP 5.0.0](https://github.com/renesas/fsp/releases/tag/v5.0.0)

Simply blink an LED

Example usage:

i.  Create build system: ```cmake -DCMAKE_BUILD_TYPE=Debug -B build```

ii. Build firmware: ```cmake --build build --target all```

iii. Use JLinkGDBServer with the following options: ```-select USB -device R7FA4M1AB -if SWD -speed auto -port 2331 -nogui```
