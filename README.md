
# Keithley 6430 CV Measurement Script

A Python script for cyclic voltammetry measurements using the Keithley 6430 Sub-Femtoamp Remote SourceMeter. The script uses PyVISA for instrument communication and implements CV measurements in batch mode.

## Features

- Automated cyclic voltammetry measurements
- Batch processing of voltage sweeps
- Data acquisition and visualization
- Key configurable measurement parameters:
  - Voltage range
  - Step size
  - Integration time (NPLC)
  - Current compliance
  - Current measurement ranges
- Data export in both text and HTML formats
- Scan rate calculation and monitoring

## Requirements

- Python 3.x
- PyVISA, PyVISA-py
- NumPy
- Plotly
- GPIB interface (NI-VISA or equivalent)

## Usage

1. Connect the Keithley 6430 via GPIB (default address: GPIB0::24::INSTR)
2. Open [`keithley.ipynb`](keithley.ipynb) in Jupyter Notebook
3. Configure measurement parameters:
   ```python
   start_voltage = -0.1  # V
   end_voltage = 0.7    # V
   step_voltage = 0.005 # V
   ```
4. Run the notebook cells sequentially and in the configuration cell change the corresponding measurement settings
