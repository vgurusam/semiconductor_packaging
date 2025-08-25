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

	Anatomy of packages
	§ Leadframe Packages: 
		§ These packages use a metal frame (typically copper or alloy) as the substrate, with leads extending outward for electrical connections. Key examples include: DIP (Dual In-line Package), QFN (Quad Flat No-leads), CSP (Chip Scale Package), QFP (Quad Flat Package).
	§ Laminate Packages: 
		§ Laminate packages use a multilayer organic substrate (e.g., epoxy-based laminates) for higher density and performance. Key examples include:
			§ Wire Bond PBGA (Plastic Ball Grid Array): This has solder ball array used to attach the substrate to the board. The gold wirebonds are used to make electrical connections for the die. 
			§ Flip Chip PBGA: Uses flip-chip technology where the die is flipped and connected via solder bumps (with epoxy underfill) to the laminate substrate, improving performance and reducing size.
			§ LGA (Land Grid Array): A flat package with contact pads instead of balls, mounted directly onto the board.
			§ FC-CSP (Flip Chip Chip Scale Package): A compact flip-chip design with solder bumps on a laminate substrate, ideal for space-constrained applications.
	§ Advanced Package Substrates
		§ 2D: Multiple dies (Die1, Die2) are mounted side by side on substrate. Connection between dies is through the substrate.
		§ 2.1D: Similar to 2D but includes an RDL layer between the dies and substrate. Improved connection between dies as it needn't go all the way to substrate.
		§ 2.3D: Similar to 2.1D but uses an organic interposer instead of RDL layer.
  		§ 2.5D: The organic interposer in 2.3D is replaced with silicon interposer which gives better connectivity. Example: CoWoS (Chip on Wafer on Substrate)

 <img width="903" height="506" alt="image" src="https://github.com/user-attachments/assets/897fb1ea-b631-47ca-ae65-71f2b730a79e" />


**Comparison of various packages**

<img width="908" height="513" alt="image" src="https://github.com/user-attachments/assets/ef13fe4a-a283-4f35-a99c-183482b9b429" />


**Module #2 : From Wafer to Package: Assembly and Manufacturing Essentials**

2.1: Supply Chain and Facilities
Supply Chain Stages: The process is divided into five main stages, each supported by specific inputs:
	
	1. Design House: Involves creating the integrated circuit layout (GDSII file) and developing test protocols using specialized software and foundry-provided design kits. 
		§ Inputs: EDA tools (Electronic Design Automation), foundry PDKs (Process Design Kits).
		§ Output: IC Design (GDSII) and Test Program.
	2. Wafer Fabrication: Manufacturing of design into a wafer die. 
		§ Inputs: Silicon wafers, equipment, gases, chemicals, materials.
		§ Output: Wafer with fabricated ICs.
	3. Package Assembly and Test: Fabricated dies are diced from the wafer, packaged (e.g., with substrates and lids), and tested for functionality for the next stage.
		§ Inputs: Substrates, tools, materials, chemicals, lids.
		§ Output: Individual ICs assembled in a package and tested.
	4. Board Assembly and Test: Packaged ICs are mounted onto a PCB, along with other components, and the board is tested for performance.
		§ Inputs: PCBs (Printed Circuit Boards), tools, materials.
		§ Output: Many packages assembled on a board and tested.
	5. Product Assembly and Test: The tested PCB is integrated into the final product (e.g., a smartphone), which undergoes final assembly and testing.
		§ Inputs: Components, tools.
		§ Output: Final product.



<img width="736" height="863" alt="image" src="https://github.com/user-attachments/assets/ef456793-2b42-4e10-8831-7fc69981af4c" />


Introduction to a Package Manufacturing Unit (ATMP)
	• What happens in ATMP? 
		§ ATMP (Assembly, Testing, Marking, and Packaging): It includes die attachment (e.g., bonding), encapsulation, electrical testing, reliability checks, marking (e.g., laser etching for traceability), and final packaging.
	• Who does ATMP?
		§ OSAT (Outsourced Semiconductor Assembly and Test): Specialized companies like ASE, Amkor, or TATA that handle ATMP for fabless or IDM firms. The ATMP process can also be performed in-house by integrated manufacturers such as Intel, TSMC, Micron, Samsung, or SK Hynix, allowing for greater control over quality and supply chain.


<img width="755" height="626" alt="image" src="https://github.com/user-attachments/assets/ae827be3-5b56-40b1-b2e2-d353aabf86b1" />

2.2 - Wafer Pre-Preparation - Grinding And Dicing
Activities Inside the Cleanroom Area
	• The process starts with incoming wafer handling and inspection, then proceeds to protective lamination. It flows downward to dicing, mounting, and grinding steps. This preparation is crucial before dies are assembled into packages, as it transforms a full wafer into individual, thinned dies ready for bonding and encapsulation. The overall process in the cleanroom prepares dies for downstream assembly, testing, and packaging in OSAT facilities.
	• Details
		§ Incoming Wafer Carrier: A stack of wafers arrive in sealed carriers (e.g., FOUPs or cassettes)
		§ Wafer Inspection: The wafer is visually and automatically inspected to filter only the good wafers to proceed. 
		§ Wafer Front Tape Lamination: A protective tape is laminated onto the front (active) side of the wafer to protect the circuits from mechanical damage during grinding and dicing. 
		§ Wafer Backside Grinding: This step removes excess silicon to thin the wafer backside and compact packaging, better heat dissipation, and 3D stacking in advanced devices. 
		§ Tape Frame Mounting to Wafer Backside: The wafer's backside is mounted onto a dicing tape within a metal or plastic frame (ring frame). This mounting provides mechanical support and stability for the wafer during dicing and handling. 
		§ Two-Step Wafer Dicing (Laser Grooving + Blade Dicing): The wafer is cut into individual dies using a hybrid method: first, laser grooving creates precise shallow cuts, followed by mechanical blade dicing to complete the separation. 
		
<img width="740" height="431" alt="image" src="https://github.com/user-attachments/assets/7ae49cd0-1bfe-4cdd-8f54-bae5b9cd86bf" />

<img width="1911" height="1040" alt="image" src="https://github.com/user-attachments/assets/93476b20-483b-4221-b777-a41cf1268680" />

2.3 - Wire Bond Packaging - Die Attach To Molding
	• The wire bond packaging process, a widely used technique in semiconductor packaging, focusing on the sequence from die attach to molding. This process is part of the back-end manufacturing in an ATMP (Assembly, Testing, Marking, and Packaging) facility and is conducted in a cleanroom environment. 
	• Steps involved
		§ Die Attach: The silicon die, separated from the wafer, is attached to a substrate (e.g., leadframe or laminate) or a die pad using an adhesive material, such as epoxy. The die being placed onto a substrate with a dispensing nozzle applying adhesive. This step provides mechanical stability and a thermal/electrical pathway between the die and the package. 
		§ Curing: The die-attached unit is subjected to a heating process to cure the epoxy, ensuring a strong and stable bond between the die and the substrate.
		§ Wire Bonding: Wire bonding connects the die's bond pads to the substrate or leadframe using thin wires (typically gold, copper, or aluminum). The process begins with the formation of a free air ball (FAB). A fine wire is fed through a capillary tool, and a high-voltage electric arc melts the wire tip to form a spherical FAB. The FAB is pressed onto the die's bond pad under heat and ultrasonic energy, creating a metallurgical bond (e.g., ball bond). The capillary then moves to the substrate, forming a wedge bond or stitch bond, and the wire is cut, completing the connection. 
		§ Molding: The assembled die, wire bonds, and substrate are encapsulated with a mold compound (e.g., epoxy resin) using a transfer molding machine. Molding protects the die and wire bonds from environmental factors such as moisture, dust, mechanical stress, and thermal shock. 
		§ Marking: It involves applying identification details to the molded package using techniques like laser etching, ink printing, or stamping. 
		§ Singulation (Dicing Blade): Singulation separates individual packaged ICs from a panel or strip (e.g., a leadframe or substrate array) into standalone units. The sawing or punching machine cuts through the molded panel along pre-defined scribe lines. These techniques are chosen based on package type (e.g., QFN, BGA) and material.



<img width="813" height="996" alt="image" src="https://github.com/user-attachments/assets/15dd2685-0da6-440e-a165-87b63895aaf4" />

2.4 - Flip Chip Assembly - Bump Formation And Underfill
Flip-Chip Packaging Process
	§ Bump Formation on Silicon: Solder bumps or copper pillars are created on the active side of the silicon die at the bond pad locations. This involves applying an under-bump metallurgy (UBM) layer followed by solder deposition.
	§ Chip Flip and Placement: The bumped die is inverted and precisely aligned with matching pads on the substrate (e.g., laminate or interposer). A pick-and-place machine positions the die, ensuring accurate alignment before bonding. 
	§ Flux Dispensing: A small amount of flux is dispensed using a dispensing tool onto the substrate pads or die bumps to remove oxides and improve solder wetting during reflow. 
	§ Solder Reflow: The assembly is heated in a reflow oven (e.g., 220-250°C) to melt the solder bumps, forming metallurgical bonds between the die and substrate. Reflow solidifies the electrical and mechanical connections, locking the die to the substrate. 
	§ Flux Cleansing: Residual flux is removed using a cleaning agent (e.g., deionized water or solvent) to prevent corrosion or contamination. 
	§ Underfill Dispensing: Liquid epoxy underfill is applied along the die edges, flowing beneath via capillary action to fill the gap between the die and substrate. Underfill reinforces the structure, compensating for thermal expansion mismatches and protecting bumps from mechanical stress or moisture ingress using a nozzle dispensing underfill.
	§ Underfill Cure: The underfill is cured with heat (e.g., 100-150°C) in an oven to harden into a solid polymer. Curing stabilizes the underfill, securing the die and enhancing reliability by preventing movement or degradation under operational conditions.
	§ Molding: The entire assembly is encapsulated with a mold compound (e.g., epoxy resin) using a transfer molding machine to protect the die, bumps, and underfill. 
	§ Marking: Identification details (e.g., part number, logo, batch code) are etched onto the molded package using laser marking or ink printing
	§ Ball Mounting and Reflow on Substrate: Solder balls are placed on the substrate’s bottom pads (for BGA packages), and the assembly is heated in a reflow oven to bond the balls, completing the package-to- board interface. 
<img width="740" height="567" alt="image" src="https://github.com/user-attachments/assets/947cd205-ba9f-475f-97d9-2340e15edc01" />

<img width="1902" height="1054" alt="image" src="https://github.com/user-attachments/assets/69d74561-8e54-4746-a304-cfada7d5692f" />

2.5 - Wafer Level Packaging And Conclusion
	§ Wafer Level Packaging (WLP) encapsulates and interconnects dies at the wafer level before singulation. 
	§ Types of WLP
		§ Fan-in WLP (FI-WLP): Interconnects are confined within the die area, limiting I/O count but ideal for compact, low-pin-count devices.
		§ Fan-out WLP (FO-WLP): Extends interconnects beyond the die area onto the package, enabling higher I/O counts and supporting complex chips like CPUs or GPUs.
			§ Reconstitution Process: Individual dies (after wafer dicing) are placed face-up on a temporary carrier (e.g., glass or tape) with a gap between them. The carrier is then overmolded with an epoxy mold compound to form a reconstituted wafer, embedding the dies. Reconstitution creates a uniform wafer-like structure from disparate dies, enabling wafer-level processing. 
			§ RDL (Redistribution Layer) Preparation: A redistribution layer is fabricated on the reconstituted wafer to reroute the die’s bond pads to desired locations for external connections. This involves depositing dielectric layers, patterning metal traces (e.g., copper), and via formation. 
			§ Solder Ball Attach: Solder balls are placed and reflowed onto the RDL pads to form the external connections (e.g., for BGA packages). Solder balls provide the mechanical and electrical interface for mounting the package onto a PCB, ensuring reliable connectivity and supporting surface-mount technology.
			§ Final Laser Marking: Identification details (e.g., part number, logo, batch code) are etched onto the package surface using a laser marking system after molding and ball attach.
			§ Singulation: The reconstituted wafer is diced into individual packages using a saw or laser along pre-defined scribe lines. Singulation separates the packaged dies into standalone units, allowing them to be picked and placed onto PCBs or shipped. 
<img width="740" height="470" alt="image" src="https://github.com/user-attachments/assets/2d228ea6-002c-4270-b8ed-958bd0dc2f81" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/227d38b8-3611-4581-b886-ad103c5aadfd" />

Module 3:  Labs for Thermal Simulation of Semiconductor Packages
In this Lab, we use ANSYS Electronic Desktop Tool (EDT) to setup a Flipchip BGA package, define material definitions and thermal sources, do thermal analysis on the package.

The IcePak tool inside the ANSYS EDT is used for doing thermal analysis. Below is a snapshot of the Labs activity.



Module 4 - Ensuring Package Reliability: Testing and Performance Validation
4.1 - Introduction to Package Testing and Electrical Functionality Checks
	§ What are the testing that happens different stages?
		§ Foundry Testing Stages
			§ Front End Manufacturing: Silicon wafers are fabricated in this step. It leads to fine tuning of the Process parameters to improve yield, reduce leakage and improve speed/ performance.
			§ Wafer Probe Test: Individual circuits on the wafer are tested using probes to check for electrical performance and identify defective dies. 
		§ OSAT Testing Stages
			§ Wafer Sorting: Wafers are sorted based on test results. Good dies are separated from defective ones and only the good dies proceed to packaging.
			§ Package Manufacturing: Involves assembling the sorted dies into packages to protect them and enable connectivity. Processes include die attachment, wire bonding, and encapsulation.
			§ Package Testing: Packaged Testing phase in semiconductor manufacturing, divided into two main areas: the Processing Zone and the Testing Area, with a sequential testing process.
		.

<img width="740" height="1072" alt="image" src="https://github.com/user-attachments/assets/bea71830-2fdd-4af0-9fb8-e25802172c73" />

Package Testing
	§ This involves Processing Zone and Testing Area steps.
		§ Processing Zone: Die bonding, wire or flip-chip bonding, encapsulation, and RDL (Redistribution Layer) formation are all handled in this step. Packages are then loaded onto a tray after singulation, for further testing.
		§ Testing Area: This step involves doing  Electrical, burn-in, and reliability chamber tests
  			§ AOST (Assembly Open and Short Test): Checks for open circuits and short circuits on the package board, using a package socket.
			§ Burn-in Test: Temperature and voltage and power cycling are elevated to accelerate ageing to catch early-life reliability issues.
			§ Final Test: Conducts cold and hot tests to validate functional, parametric, reliability and validate the electrical performance of the packaged IC across temperature and voltage corners and ensure it meets the datasheet specifications.
<img width="654" height="138" alt="image" src="https://github.com/user-attachments/assets/f0ac9c2a-1605-408f-a63e-d0c97aa50379" />


<img width="740" height="118" alt="image" src="https://github.com/user-attachments/assets/4c38ee6b-c007-4d48-a369-fef9491fe5dc" />

<img width="1904" height="1056" alt="image" src="https://github.com/user-attachments/assets/ea645549-0697-4b12-bcc0-999b517bb065" />






