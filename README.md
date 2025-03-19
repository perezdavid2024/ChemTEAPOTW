# ChemTEAPOTW

![image](https://github.com/user-attachments/assets/6e8bc267-effa-4165-a5eb-7382fde270e6)


## Overview
The Chemical Tracker and Exposure Assessor in Publicly Owned Treatment Works (ChemTEAPOTW) model integrates frameworks for conventional treatment processes, chemical fate and transport across treatment stages, and occupational exposures (dermal and inhalation). The model employs a steady-state open-loop approach to predict chemical partitioning across unit processes like leading to emissions to air, water discharges, or land application of byproducts.

## Requirements
This code was written using Python (https://www.python.org/downloads/) and Windows operating system. The following Python libraries are required for running the code:

1. numpy (https://pypi.org/project/numpy/)
2. scipy (https://pypi.org/project/scipy/)
3. pandas pandas (https://pypi.org/project/pandas/)


## Model Use
The ChemTEAPOTW simulates a chemical partioning through a standard POTW, with a primary clarifier (900m3), five stage nutrient removal aeration tanks in series (2 anoxic @ 1500 m3 and 3 aerobic @ 3000 m3), secondary 
clarifier (1500m3), unitless dewatering and sludge thickening units, and a 3000 m3 anaerobic digester. The plants is run @ steady state with several recylced flows and an approximate input flow rate of 20648 m3/d. The 
plants design has been adopted from the Benchmark Simulation Model (BSM2) (http://iwa-mia.org/wp-content/uploads/2018/01/BSM_TG_Tech_Report_no_3_BSM2_General_Description.pdf).

1. Input chemical concentration (SCH_inf 0 [mg/L]) on Line 30
2. Remove commented status from chemical list (starting on line 378), or add chemical to list using Comptox info for henry's constant, Octanol Partition Coefficient, Molar Mass, Density.
3. Indicated whether a chemical is biodegradable using bio = 1 for yes or 0 for no.
4. Run the model.


## Output
After running the Python script you obtain an output text outlining the operating conditiopns of the plant (flow rates [m3/d], retention times [d-1], food-to-mass rations[-], etc.) as well as chemical concentrations, in both liquid and solid forms, of the chemical of interest. An example opf the text is included in the "POTW_dataset.xls" file.


## Disclaimer
The views expressed in this article are those of the authors and do not necessarily represent the views or policies of the U.S. Environmental Protection Agency. Any mention of trade names, products, or services does not 
imply an endorsement by the U.S. Government or the U.S. Environmental Protection Agency. The U.S. Environmental Protection Agency does not endorse any commercial products, service, or enterprises.

##Acknowledgement
This research was supported in by an appointment for David Perez to the Research Participation Program at the Center for Environmental Solutions and Emergency Response, Office of Research and Development, U.S. 
Environmental Protection Agency, administered by the Oak Ridge Institute for Science and Education.
