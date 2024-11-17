# Ex No: 01     Design & Implementation of CMOS Inverter Design Using Cadence EDA Tools   

## Aim:
To design and implement a CMOS inverter circuit using Cadence EDA tools, analyse its electrical characteristics, and understand the fundamental principles of CMOS technology, including the design process, layout, and simulation techniques.

## Tools Required:
* Personal Computer
* Cadence Virtuoso Software

## S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
## Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


## i)	Procedure for Creating New Library.
1.	File –New – Library
2.	Name: Give name for ur library Ex: VLSILAB_EXP_1
3.	Enable Attach to an existing technology library, Click OK
4.	Attach the library to the technology library gpdk045.Click OK

## ii)	Create Schematic Cell view.
1.Go to 1st window i.e virtuoso (CIW)
  * File-New-Cell view
  * Setup the new file form
2.Library: Select the one you created.
3.Cell: Give the experiment name Ex: Inverter ViewSchematic
4.Type: Schematic press OK
  *Add the required components from the libraries and make the connections.
5.	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
6.	Click on browse. This opens the library browser
7.	Now select the appropriate library for components like 
8.	Gpdk45 ------------------------nmos1v, pmos1v
9.	Create Input and Output pins
10.	Make the connections by using fixed narrow wire key
11.	Click Check and Save button
![Screenshot 2024-09-12 104323](https://github.com/user-attachments/assets/ada97677-830b-4de5-acbe-16e8d45d9e00)

## iii)	Creating the Symbol for schematic Cell view

* In the schematic window, execute 
  - Create – Cell view – From Cell view
  -   The cell view from cell view window appears
  -   Check Lib Name, Cell Name, From View name must be schematic Press ok
*	Now Symbol generation form appears. Click Ok If No changes required
*	A new window with with default symbol is created.
*	Edit the symbol if you want to give actual symbol shape else continue.
*	Execute Create-Cell view-from cell view
*	Library Name and Cell Name must be same which you have used for schematic. Press OK
*	Check for the position of pin side.Prss OK
*	Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot 2024-09-12 104421](https://github.com/user-attachments/assets/a7ec4b0d-3a60-426c-a1e8-a9b28ff9fea0)


## iv)	Creating the new test cell view

* Go to CIW window, Execute File-New-Cell view
  - Setup the new file form
  - Library: Select the one you created.
  - Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
  - View: Schematic
  - Type: Schematic press OK
* Follow the step 3(ii) d to make the required connections
![Screenshot 2024-09-12 104451](https://github.com/user-attachments/assets/d972edbc-2e0c-4d07-b12f-0acff691e009)

## Analog simulation by SPECTRE.
* In test cell view window
* Launch – ADE L(Analog Design Environment)
  - Execute Setup—Simulation/directory/Host A new window opens
  - Set the simulation window to spectre and click ok
  - Execute Analysis – Choose. A window opens.
  - Select the type and set the specifications and press OK
  - Execute Output s—to be plotted – Select on Schematic
  - Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
* Execute Simulation -- Net list and Run

## For Transient Analysis Settings and Output

![Screenshot 2024-09-12 104602](https://github.com/user-attachments/assets/df643427-263a-4e31-84bb-48a0990a6814)

![Screenshot 2024-09-12 104645](https://github.com/user-attachments/assets/778d7f42-34fd-4bdb-834b-2d18649bdcd5)

## For DC Analysis Settings and Output
![Screenshot 2024-09-12 104753](https://github.com/user-attachments/assets/c14e57c6-996c-4b20-bbbb-6ee67e3159d0)

![Screenshot 2024-09-12 104802](https://github.com/user-attachments/assets/9d38f5cf-cde8-4b8b-b981-4b6f2ab16ede)

 

# Results:
1.	Successfully designed the CMOS inverter schematic using Cadence EDA tools.
2.	The simulation results demonstrated the correct logic operation of the inverter, where the output voltage switches between high (Vdd) and low (0V) levels, corresponding to the input voltage transitions.
3.	The Voltage Transfer Characteristic (VTC) curve was plotted, showing the relationship between input and output voltages.
