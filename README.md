# masters-thesis
TET4900 Electrical Energy and Energy Systems, master's theis

# Master's Thesis Repository – Spring 2025

This repository contains the Python code developed for our master's thesis at NTNU during the spring of 2025.

## Overview

The thesis investigates three scenarios for capacity reserve dimensioning methodologies:
- **Base Case**
- **Upper Bound**
- **Lower Bound**

Each scenario is analyzed for two target years: **2024** and **2050**.

## Structure

- **`2024_Data/`** and **`2050_Data/`**  
  Contain input data for each respective year.  
  The datasets were created specifically for this thesis using historical data for 2024 and projected data for 2050.

- **`Calc_reserve_req_2024.py`** and **`Calc_reserve_req_2050.py`**  
  Calculate scenario-specific capacity reserve requirements for each year.  
  The results are saved as CSV files and can be used for further analysis or plotting.

- **`BaseCase_2024.py`, `UpperBound_2050.py`, etc.**  
  Each script runs the market-clearing model for a specific scenario and year.  
  These scripts take input from the corresponding data folder (`*_Data/`) and generate the required sets and parameters, following the mathematical formulation presented in the thesis.

## Usage

To run a specific scenario:

1. Ensure that the input data is available in either the `2024_Data/` or `2050_Data/` folder.
2. Run the corresponding reserve requirement calculation script (e.g., `Calc_reserve_req_2024.py`).  
   This will output final up/down reserve requirement files (e.g., `Final_up_reserve_BaseCase.csv`).
3. Run the market-clearing script for the scenario (e.g., `BaseCase_2024.py`).  
   This will produce result files used for evaluation and visualization.

## Output

Each script generates output files in CSV format, which can be used for:
- Post-processing and analysis
- Plotting reserve requirements over time
- Evaluating scenario-specific system cost and market outcomes
- Evaluating hydropower usage 

