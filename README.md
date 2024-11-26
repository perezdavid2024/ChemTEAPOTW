# ChemTEAPOTW

![image](https://github.com/user-attachments/assets/6e8bc267-effa-4165-a5eb-7382fde270e6)


## Overview
The Chemical Tracker and Exposure Assessor in Publicly Owned Treatment Works (ChemTEAPOTW) model integrates frameworks for conventional treatment processes, chemical fate and transport across treatment stages, and occupational exposures (dermal and inhalation). The model employs a steady-state open-loop approach to predict chemical partitioning across unit processes like leading to emissions to air, water discharges, or land application of byproducts.

## Requirements
1. Python
2. numpy
3. scipy
4. pandas
5. math

## Model Use
1. Input chemical concentration (SCH_inf 0 [mg/L] on Line 30
2. Remove commented status from chemical list (starting on line 378), or add chemical to list using Comptox info for henry's constant, Octanol Partition Coefficient, Molar Mass, Density.
3. Indicated whether a chemical is biodegradable using bio = 1 for yes or 0 for no.
4. Run the model.
