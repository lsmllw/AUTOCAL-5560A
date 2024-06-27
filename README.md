Automated Calibration of Electrical Quantities with Fluke 5560A

This project implements an automated system for the calibration of various electrical  using the Fluke 5560A calibrator, through IEEE-488 protocol. The application allows for automated calibration of voltage and current sources and meters, as well as resistors and capacitors, among others, with results stored in an Excel spreadsheet.

Features
Automatic calibration of:
AC and DC Voltage Sources
AC and DC Current Meters
AC and DC Current Sources
DC Voltage Meters
AC and DC Resistance Meters
Standard Resistors and Decade Resistors in AC and DC
DC Current Shunts
Capacitance Meters
Active and Reactive Power Meters
AC and DC Power Sources
Phase Angle and Power Factor (cos φ) Meters
Graphical user interface for ease of use
Results stored in Excel spreadsheets

Python libraries:
tkinter
pyvisa
openpyxl

Installing the Libraries
pip install pyvisa openpyxl tkinter

Usage
Steps to Run the Application
Conect the instrument to the calibrator, both IN and OUT terminals, for the equipment to realize both writing the reference value, and reading the output to the measured instrument. 

Save the code in a file, for example, calibration.py, and run it using Python

The interface allows the user to select the quantity to be calibrated, enter measurement points, the Excel file path, and the name of the sheet where the results will be saved.

The application communicates with the calibrator via GPIB using the pyvisa library.

Based on the selected quantity, the application configures the calibrator, performs multiple readings, calculates the average of the measured values, and compares them with the expected values.

Calibration results are stored in an Excel spreadsheet at the path specified by the user, to calculate the uncertain and other calibration parameters.
