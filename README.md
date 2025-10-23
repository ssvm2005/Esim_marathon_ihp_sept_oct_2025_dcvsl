# Esim_marathon_ihp_sept_oct_2025_dcvsl
1-Bit Full Adder Implementation Using DCVSL (Differential Cascode Voltage Switch Logic) High-speed, low-power full adder circuit designed using Differential Cascode Voltage Switch Logic (DCVSL). The project demonstrates efficient logic design for arithmetic circuits in VLSI with reduced transistor count and minimal static power dissipation.

This project presents the design and analysis of a 1-bit Full Adder using Differential Cascode Voltage Switch Logic (DCVSL).
The design focuses on achieving:
  -> High-speed operation
  -> Low power consumption
  -> Area efficiency
DCVSL provides both true and complementary outputs with minimal static power dissipation, making it an ideal choice for arithmetic building blocks in VLSI systems.
The project is build using Open Source Tools like eSim and Ngspice. The objective of the marathon was to implement circuits using IHP-SG13G2. The attached output waveforms include the default esim nmos,pmos 180nm mosfets. The .cir.out file used for IHP-SG13G2 is also attached.

<img width="523" height="326" alt="image" src="https://github.com/user-attachments/assets/1d530cdc-6c15-46f7-9a37-a54ba7efe3c6" />

Fig 1: Circuit Diagram

<img width="1059" height="710" alt="image" src="https://github.com/user-attachments/assets/6bf33259-c5ce-455f-9881-dc1f37c27ec7" />
Fig 2: DCVSL SUM circuit implemented in eSim

<img width="1100" height="689" alt="image" src="https://github.com/user-attachments/assets/d4f43757-6fa9-4c58-97fe-5dc1d96a05f2" />
Fig 3: DCVSL CARRY circuit implemented in eSim

One also create cmos inverter subcircuit in eSim and create input for Abar,Bbar and Cbar.
Load Capacitance is 0.01uF was added in CMOS circuits to model the effect of parasitic and fan-out capacitances present at the output node, allowing accurate analysis of propagation delay, power consumption, and realistic output waveforms during switching.


<img width="1852" height="688" alt="Screenshot 2025-10-23 082759" src="https://github.com/user-attachments/assets/f0bfd82b-73eb-4bdc-9d49-5f51e239c3a7" />

Fig 4: Adding Simulation Parameters

One can change the details in .cir.out file after converting KiCad to Ngspice file to include IHP PDK file. I have added the text in cir_out_file.txt attached in the gitnub. 

After plotting the Ngspice graph:

The OUTPUTS ARE:
<img width="700" height="823" alt="out_sum_final" src="https://github.com/user-attachments/assets/f4e96587-200a-4ddd-b926-0cf87a3f5b23" />

Fig 5: Output for Sum - Blue line represents the output - rest are A,B,C bit values

<img width="700" height="823" alt="out_carry_final" src="https://github.com/user-attachments/assets/4393d3e3-1e9c-417e-b783-e8b065750dba" />

Fig 6: Output for Carry - Blue line represents the output - rest are A,B,C bit values

<img width="384" height="357" alt="image" src="https://github.com/user-attachments/assets/b88c2d7b-3a3b-46c4-bf99-14ad0ca07fbd" />

Fig 7: Truth Table for the logic implemented

References:
https://www.researchgate.net/publication/311418018_A_Novel_1-Bit_Full_Adder_Design_Using_DCVSL_XORXNOR_Gate_and_Pass_Transistor_Multiplexers

https://esim.fossee.in/home

https://github.com/IHP-GmbH/IHP-Open-PDK/tree/main

https://ngspice.sourceforge.io/download.html

Hackathon Description:
The eSim Marathon – Circuit Design & Simulation with IHP SG13G2 is a nationwide competition organised by FOSSEE (IIT Bombay) that invites participants to design and simulate analog, digital or mixed-signal circuits using the open-source EDA tool eSim and the open-source 130 nm BiCMOS PDK IHP Microelectronics SG13G2. The goal is to democratise VLSI design education and provide hands-on experience with real world PDKs and tools.  FOSSEE

Participant Details:
S S V Mridula,
Pre-Final Year Student, B.Tech Electronics and Communication Engineering
Vellore Institute of Technology, Chennai Campus
