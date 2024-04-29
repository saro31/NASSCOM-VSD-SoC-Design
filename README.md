NASSCON – VSD SoC Design Program [24 April – 7 May 2024] is a two-week hands-on workshop that helps to understand RTL2GDSII flow and SoC design flow. 

Day 1 - Inception of open-source EDA, OpenLANE, and Sky130 PDK

Day 1.1 - SKY130_D1_SK1 - How to talk to computers

SKY_L1 - Introduction to QFN-48 Package, chip, pads, core, die, and IPs
In general, the entire electronic gadget contains a microprocessor or microcontroller as a CPU in the motherboard PCB. The following Arduino board contains a microcontroller ATmega328P chip as highlighted in the figure. This microcontroller is packaged with QFN-48 with a surface mount.
 
The following diagram shows the dimensions of the QFN-48 package with 7 mm × 7 mm.
 
To understand the concept of Die, Pads and Core design is provided in the following diagram. 
Die – In the Integrated Circuits (IC), the overall functional circuit or core is fabricated in a small dimension. 
Pads – The core function needs to connect with the external world in terms of providing the input and getting the output. 
. 
Further, the package contains two major modules named as Macros and Foundry IPs. Macros are known as pre-defined circuits with proper verification and in Foundry IPs is designed for the required design from the customer for specific applications. 
 
SKY_L2 - Introduction to RISC-V
One of the popular Open Standard  - Instruction Set Architecture (ISA) is known as RISC-V architecture which comes with free royalty licenses. The following figures show how a C-program (RISC-V architecture) helps to implement the Picorv32 CPU core and finally with hardware layout.  
 

SKY_L3 - From Software Applications to Hardware
The elaborated flow is given below by highlighting from initial application software stage to the hardware layout with various conversion stages. In the system software, the C / C++ code was compiled and assembly code, and then with the help of the assembler, the final binary code was generated and given as input to the hardware design layout. 
In summary, the initial process starts with ISA, then RTL Synthesis (CPU- Picorv32), and finally Physical design (layout). 
 

Day 1.3 - SKY130_D1_SK2 - SoC design and OpenLANE
SKY_L1 - Introduction to all components of open-source digital ASIC design
OpenlLANE is a popular environment, which integrates various EDA tools to support from RTL to GDSII form. This arrangement integrates three major domains known as EDA Tools (Qflow, OpenROAD), PDK Data (Skywater130nm), and RTL Design (Github.com) to achieve efficient ASIC flow.
 
SKY_L2 - Simplified RTL2GDS flow
RTL2GDSII flow has a lot of technical stages known as Synthesis, Floor Planning, Placement, Clock Tree Synthesis, Routing, and Final Sign. 
Synthesis – It is the process of converting RTL code (Verilog / VHDL) into required Standard Cell Libraries (SCL) and it is known as Netlist of the design.
Floor Planning – The next stage of synthesis is known as floor planning, which allocates different design blocks and connects them with proper pads. Macro floor planning and power planning are considered as very important processing of floor planes.
Placement – This process helps for better placement of the cells on the proper floor plan and aligned with the available design space. This process is considered for global and detailed placement.
Clock Tree Synthesis – It helps to deliver the master clock to all the required sequential blocks like flip flops in terms of Tree structure.
Routing – This process is used to interconnect the design with various metal layers as per the requirement and availability. 
Sign Off – This stage contains Physical verification (DRC and LVS) and Timing verification (STA)
 
	

