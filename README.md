# Description

The Microsoft Excel workbook "CLP Spreadsheet Solver" is an open source tool for representing, solving, and visualizing the results of Container Loading Problems (CLPs), also known as 3D Bin Packing Problems.

The users can enter the dimensions of item types and containers in associated worksheets, find a heuristic solution through an LNS algorithm, visualize the solution in 3D, and animate the loading plan.

The users can follow the numerical order of buttons in the dedicated CLP Spreadsheet Solver tab, filling in data to the green cells. Yellow cells are computed by Excel. Light blue cells are the solution to be found by the solver (or input by the user). Cells that turn red signify an error.

A two-minute tutorial video is available at https://youtu.be/-0MCkd-CjD0

The details of the solution algorithm are provided in this open-access paper: https://www.sciencedirect.com/science/article/pii/S0305054823000631

The file will work on Microsoft Excel 2007 or newer versions that work locally. It is not tested for the online versions of Excel. 

The solver works much faster in the Windows versions of Excel. It also works faster if the file is saved as a binary Excel file, e.g. `CLP_Spreadsheet_Solver.xlsb`.

The macros should be enabled for the functionality. If the macros are disabled due to security settings, they can be enabled by right-clicking the solver file in File Explorer, and then navigating to Properties->General, and ticking the `Unblock` box.

You can send comments and questions to the project manager: G.Erdogan@bath.ac.uk

# Version history:

## Version 1.6

Users can now animate the loading plan and the unloading plan.

## Version 1.55

Users can now select the unit of weight and length from the console worksheet. All items and containers should be declared using the same units. For example, if the items are declared in feet and kg, so should the containers be.

## Version 1.5

Users can now set the language of the menu and the rest of the interface from the console worksheet. The available languages are: Turkish, German, Spanish, Italian, French, Portuguese, Arabic, Indonesian, Urdu, Bengali, Swahili, Persian, and Malay. Special thanks to Rusuhi Cantay for his help with multi-language support.

## Version 1.4

Further improvements to the solver, and minor bug fixes.

## Version 1.3

The solver has been improved, and also minimizes the moment with respect to the z-axis (i.e. approximately equal load for the right and left sides of the container) for balanced load.

## Version 1.2

The users now can define item types to be "heavy" or "fragile". "Heavy" items can only be placed at the floor level, since placing them on any other item will result in the other item being damaged. "Fragile" items cannot vertically support any item (i.e. it is not allowed to place any item on top of them), no matter its weight. An item type can be both "heavy" and "fragile" simultaneously.
