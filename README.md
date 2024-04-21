# Digital-VLSI-SoC-Design-and-Planning

## Section 01 - Inception of open-source EDA, OpenLANE and Sky130PDK


A typical embedded system / electrical computer / logic would contain a central processor / logic as follows. In general it is known as a chip. However, there is more to explain. The following image shows how different interconnects, and peripherals are connected to the central processor. 

![[Pasted image 20240420214959.png]]

However, if the processor is a package which will contain a different set of peripherals as follows:

![[Pasted image 20240420215043.png]]

This specific package is a QFN-48 package. QFN stands for Quad Flat No-leads. There are other [[IC packages]] and are categorized into following package types:
1. [[Through-Hole Mount Packages]]
2. [[Surface Mount Packages]]
3. [[Chip-Scale Packages]]
4. [[System-in Package]]
5. [[Multi-Chip Modules]]
6. [[Leadless Packages]]
QFN is an example for leadless packages. The QFN package in this case is $7 \ \text{nm} \ \times \ \text{nm}$ .
![[Pasted image 20240420215117.png]]

The main functions of an IC package are:
* Providing mechanical support and protection
* Providing thermal and electrostatic protection
* Provide an interface for the external components to connect with the chip

A chip is connected with the external interface of the package by using two different methods. They are:
* [[Wirebonding]]
* [[Flipchip]]
The following image shows how a chip is interconnected using the wire bonding method.

![[Pasted image 20240420215205.png]]

#### Components of a chip
The following image shows the main three components of a typical chip.
* Pads: Pads are responsible for making electrical connections with the package.
* Core: The core is the chip area where all logic lies.
* Die: The die is the boundary which defines the chip area. It determines the size of the chip.
![[Pasted image 20240420215307.png]]
The following image shows a detailed view of a typical RISC-V chip SoC. It contain foundry IPs and Macros. Macros are purely logic custom built aligning user requirements. On the other hand, foundry IPs are complicated designs involving some degree of intelligence.

![[Pasted image 20240420221230.png]]

### Introduction to RISC-V 
