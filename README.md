This repository contains code for a resistance temperature coefficient measurement system, which can be used to calibrate automated computer systems that measure electrical assemblies in environments that could cause temperatures to change. For example, if you're testing electrical systems near freezers or furnaces, it can affect your measurements.

The system works by taking measurements of the electrical resistance of a material at two different temperatures, using a precision electrical measurement device. The temperature coefficient of resistance (TCR) is then calculated as the percentage change in resistance per degree Celsius. The TCR can be used to predict the resistance at a specific temperature, using the following formula:

TCR = (R2 - R1) / (T2 - T1) * (100 / R1)

Where R1 and R2 are the electrical resistances at temperatures T1 and T2, respectively.

In addition to the TCR measurement system, we have also developed a function for measurement uncertainty. This is important because all measurements have some degree of uncertainty, due to various factors such as equipment precision and environmental conditions. The function generates a random number within a specified range, which represents the uncertainty of the measurement. The range is based on a 95% standard deviation, which means that there is a 95% chance that the generated number will fall within 1 standard deviation of the mean (0).

To use the measurement uncertainty function, simply input your measurement uncertainty (in Ohms) as a variable. The function will automatically double the input value to account for the K2 Standard Deviation 17025 compliance. Make sure to use the correct units of measure, as incorrect units can lead to serious errors in your calculations.

We hope that this code will be useful for those looking to calibrate their computer systems using NIST traceable equipment.

Testing Procedure: 

To perform the testing procedure using the Ohm Temperature Calibration Tool:
Gather the necessary equipment, including a calibrated Ohmmeter, the material to be tested, and a computer running the Ohm Temperature Calibration Tool code.
Measure the resistance of the material at the low end of the temperature range, using the Ohmmeter. 

If you're a beginner to R, use this program to run the code: https://www.mycompiler.io/

Take at least 10 measurements to test repeatability.

Record the measurements and calculate the average resistance, using the Ohm Temperature Calibration Tool code. This will be the "Low Test Resistance Average" (Ro).

Measure the resistance of the material at the high end of the temperature range, using the Ohmmeter. Take at least 10 measurements to ensure repeatability.

Record the measurements and calculate the average resistance, using the Ohm Temperature Calibration Tool code. This will be the "High Test Resistance Average" (RT).

Calculate the temperature coefficient of resistance (TCR) using the Ohm Temperature Calibration Tool code, using the following formula: TCR = (RT - Ro) / (T - To) * (1 / Ro), where T is the high test temperature average, To is the low test temperature average, RT is the high test resistance average, and Ro is the low test resistance average.

Use the TCR to predict the resistance of the material at a specific temperature, using the Ohm Temperature Calibration Tool code. The program has a loop function that will give you a list of the temperature and the corresponding resistance measurements.

Use the results of the predicted resistances to calibrate automated computer systems that measure electrical assemblies in environments with moving temperatures. The goal is to make sure the software systems have efficient error budgets programmed correctly.  
