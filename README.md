
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
