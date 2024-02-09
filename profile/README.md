# The Angry Goose Initiative

[Take me to the wiki](https://github.com/angry-goose-initiative/wiki/wiki)!

# So what is AGI?

The goal of the AGI is to create a softcore RISC-V CPU that’s capable of running the Linux kernel!

# [IRVE](https://github.com/angry-goose-initiative/irve)

**[IRVE](https://github.com/angry-goose-initiative/irve)** is the first step on our journey. The plan is to use it to better understand the RISC-V architecture (with a focus on Volume 2 in particular). **If you're interested messing around with the project, this is a great place to start!**

# [LETC](https://github.com/angry-goose-initiative/letc)

We're now wrapping up the emulator and are currently in the design phase of our SystemVerilog hardware implementation called **[LETC](https://github.com/angry-goose-initiative/letc)**! It will be a 6-stage in-order pipelined design, targeting the Cora Z7 devboard containing a Zync 7000 FPGA. It will have TLBs, caches, a hardware page table walker, and will accesses peripherals and memory over an AXI interconnect of our own making!

# [RVSW](https://github.com/angry-goose-initiative/rvsw)

Our RISC-V software, including test programs, experiments, C and C++ runtime environments, bootloaders, and an SBI implementation, can be found in the **[RVSW](https://github.com/angry-goose-initiative/rvsw)** repository. We try to keep these programs as hardware-agnostic as possible, allowing IRVE and LETC to specify how things should be linked together and how hardware should be accessed. You're welcome to use it as well in your own project: just modify the example config!

# [Conductor](https://github.com/angry-goose-initiative/conductor)

**[Conductor](https://github.com/angry-goose-initiative/conductor)** is the glue that will allow LETC to chug along with ease! It is in two parts: a CLI frontend running on a host computer, and a component running on the ARM core in the Zync 7000 FPGA. It will facilitate loading test binaries and kernels into memory for LETC, managing PL clocks and resets, and coordinating I/O between the host and our our design. Lots of work ahead on this front!

# Linux-y Stuffs!

We also maintain a fork of the kernel [here](https://github.com/angry-goose-initiative/linux), and have tools to automate setting up a Linux image for AGI project in the [build-linux](https://github.com/angry-goose-initiative/build-linux) repo.

# Pronunciation

IRVE and RVSW both have each letter sounded out.

LETC on the other hand is pronounced "let-see" or "letsy"!

Conductor is, well, just the regular word lol.

# Acronyms

IRVE stands for the Inextensible RISC-V Emulator.

LETC stands for the Little Engine That Could (run Linux)!

RVSW stands for RISC-V Software. The more boring one of the bunch in terms of naming

Conductor, not being a four-letter-acronym, is new territory for us.
