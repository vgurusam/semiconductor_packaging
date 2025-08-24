# semiconductor_packaging
NASSCOM Semiconductor Packaging Course
Module 1: Packaging Evolution: From Basics to 3D Integration

1.1. Introduction To Semiconductor Packaging And Industry Overview

	• The chips are manufactured in a highly protected and clean environment. The chips usage is in real world which won't be same as its protected manufacturing environment. 
	• The purpose of semiconductor packaging is to give protection of the semiconductor devices in the die and to enable the interaction of one die to other dies/components in the outside world.
	• In a fundamental level, a packaging will have
		○ Die - Main semiconductor chip containing integrated circuits
		○ Substrate - The base layer where the die sits on. It is also called as carrier. It includes the trace and contact points for external connections
		○ Die Attach - Adhesive material used to attach Die to Substrate
		○ Wire/Solder bond - Bonding to have chip connections to outside world
		○ Molding Compound - Protective encapsulant (epoxy material) that surrounds die and wire bonds.
		○ Trace - Conductive pathways on substrate for having electrical connections.

  <img width="908" height="459" alt="image" src="https://github.com/user-attachments/assets/d8b48893-e237-4002-9b3a-32bca24b8b77" />

  		○ Where does packaging fits in the Semiconductor manufacturing?
			§ The Packaging fits in the OSAT/ATMP stage of semiconductor manufacturing.
			§ IDM - Integrated Device Manufacturing Companies are those that do the complete design, wafer manufacturing, packaging, test & assembly. Ex - Intel, Samsung etc
			§ Fabless - Companies that do only Design and do the manufacturing with other companies Ex - Apple, Nvidia, AMD etc
			§ Foundry - Companies that does wafer manufacturing for fabless companies. Ex. TSMC
			§ OSAT - Outsourced Semiconductor Assembly and Test
				□ These companies handle the wafer testing, packaging and package testing. Ex. ASE, Amkor, JCET etc.
			§ Main stages of the Back-End Process
				□ Design: Here the semiconductor circuit is conceptualized and designed by fabless or IDM companies. This involves creating the blueprint for the integrated circuit.
				□ Wafer Process: Manufacturing of silicon wafers based on the design blueprint. Conducted by foundries using advanced lithography and doping techniques.
				□ Package & Test: A critical stage where the bare dies are packaged and tested for functionality.
					® Wafer Test: Individual dies on the wafer are tested for defects to ensure they meet performance standards.
					® Package: The tested dies are encapsulated in protective packages.
					® Package Test: The packaged chips undergo final testing to verify reliability and performance under various conditions.
				□ Assembly: The final stage where the packaged chips are integrated into the final product (e.g., mounted on a PCB for devices like smartphones or computers). This step is often handled by OSATs or system integrators.
			
		
		<img width="907" height="453" alt="image" src="https://github.com/user-attachments/assets/793e4073-99fc-4407-8571-e46fd11b98cf" />

		
	
	
	1.2.Understanding Package Requirements And Foundational Package Types
	
	The package requirements revolve around selecting a design that matches the chip's functionality, provides adequate connectivity, manages heat, fits the physical space, ensures long-term reliability, and remains cost-effective. Some of the key things that affect the deciding on package are as follows:
		§ Application: The specific function of the chip defines the package requirements. If it is logic (microprocessors), memory (DRAM) or power management IC have different needs and accordingly packaging can be decided.
		§ Pin Count (I/O pins): The number of I/O pins in the chip impacts the package decision. Higher pin counts require packages like BGA or QFP.
		§ Thermal Dissipation: The heat from the chip if not properly dissipated can damage the chip and package decision depends on that. 
		§ Form Factor: The package size and shape must align with the board's layout and the device's physical constraints. 
		§ Reliability and Durability: The package must withstand environmental stresses (e.g., temperature fluctuations, humidity, mechanical shock) over its lifecycle. 
Cost: The package design must balance performance with manufacturing and material costs.

<img width="909" height="454" alt="image" src="https://github.com/user-attachments/assets/4d01ad79-cb01-47db-a6ad-4547773db2d5" />

	Package Types
	§ Through-hole Mounting:
		§ DIP (Dual In-line Package)
		§ TO (Transistor Outline)
		§ PGA (Pin Grid Array)
		
	§ Surface Mount Technology (SMT)
		§ QFN (Quad Flat No-leads): Flat package with exposed pads on the bottom for surface mounting.
		§ QFPP (Quad Flat Package): Similar to QFN but with extended leads on all four sides.
		§ CSP (Chip Scale Package): Ultra-compact, nearly the size of the die itself.
		§ PBGA (Plastic Ball Grid Array): Uses a plastic substrate with an array of solder balls.
		§ LGA (Land Grid Array): Flat contacts instead of balls, used in high-performance CPUs.
		§ PoP (Package on Package): Stacks packages vertically for memory and logic integration.
		§ MCM (Multi-Chip Module) - Intel Broadwell: Integrates multiple dies in one package for higher density.
		§ CoWoS (Chip on Wafer on Substrate) - Nvidia H100: Advanced 3D packaging with multiple chips on a silicon interposer, used in high-performance GPUs like the Nvidia H100.

<img width="1913" height="1060" alt="image" src="https://github.com/user-attachments/assets/2c01916e-a9b5-43e6-9944-4c48ab09a717" />






