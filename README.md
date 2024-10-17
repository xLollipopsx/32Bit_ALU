# 32Bit_ALU Simulation

# Aim: 

Write a verilog code for 32 bit ALU supporting four logical and four arithmetic operations,use case statement and if statement for ALU behavioral modeling.

	To Verify the Functionality using Test Bench.

# Tool Required:

	Functional Simulation: Incisive Simulator (ncvlog, ncelab, ncsim)

# Design Information and Bock Diagram:

The ALU will take in two 32-bit values, and control line. An Arithmetic unit does the following task like addition subtraction, multiplication and logical operations. As the input is given in 32 bit we get 32 bit output. The arithmetic will show only one output at a time so a selector is necessary to select one of the operator.

![image](https://github.com/user-attachments/assets/e574788c-253f-46da-8468-298fe2844f7a)

                          # Fig 1 : Block Diagram of 32 Bit ALU 

# Creating a Work space :

	Create a folder in your name (Note: Give folder name without any space) and Create a new sub-Directory name it as Exp3 or alu_32bit for the Design and open a terminal from the Sub-Directory.

# Creating Source Codes 

	In the Terminal, type gedit <filename>.v (ex: gedit alu_32bit.v). 

	A Blank Document opens up into which the following source code can be typed down. 

# Note : File name should be with HDL Extension

# a)To Verify the Functionality using Test Bench

# Source Code – Using Case Statement :

(Include program here)

	Use Save option or Ctrl+S to save the code or click on the save option from the top most right corner and close the text file.

# Creating Test bench:

	Similarly, create your test bench using gedit <filename_tb>.v or <filename_tb>.vhdl to open a new blank document (alu_32bit_tb_case).

# Test Bench :

(Include test bench program here)

	Use Save option or Ctrl+S to save the code or click on the save option from the top most right corner and close the text file.

# Functional Simulation: 

	Invoke the cadence environment by type the below commands 

	tcsh (Invokes C-Shell) 

	source /cadence/install/cshrc (mention the path of the tools) 

      (The path of cshrc could vary depending on the installation destination)
      
	After this you can see the window like below 




                          # Fig 2: Invoke the Cadence Environment

	To Launch Simulation tool 

•	linux:/> nclaunch -new& // “-new” option is used for invoking NCVERILOG for the first time for any design 

                                      or

•	linux:/> nclaunch& // On subsequent calls to NCVERILOG 


	It will invoke the nclaunch window for functional simulation we can compile,elaborate and simulate it using Multiple Step .


                               # Fig 3: Setting Multi-step simulation

	Select Multiple Step and then select “Create cds.lib File” as shown in below figure 

	Click the cds.lib file and save the file by clicking on Save option 


                                # Fig 4:cds.lib file Creation

	Save cds.lib file and select the correct option for cds.lib file format based on the HDL Language and Libraries used. 

	Select “Don’t include any libraries (verilog design)” from “New cds.lib file” and click on “OK” as in below figure .

•	We are simulating verilog design without using any libraries 

•	A Click “OK” in the “nclaunch: Open Design Directory” window as shown in below figure 

![image](https://github.com/user-attachments/assets/d5202b97-ee5c-4e0e-9eaf-5f3fa733e546)

                              # Fig 5: Selection of Don’t include any libraries

	A ‘NCLaunch window’ appears as shown in figure below

	Left side you can see the HDL files. Right side of the window has worklib and snapshots directories listed. 

	Worklib is the directory where all the compiled codes are stored while Snapshot will have output of elaboration which in turn goes for simulation .

	To perform the function simulation, the following three steps are involved Compilation, Elaboration and Simulation. 

                               # Fig 6: Nclaunch Window








      







