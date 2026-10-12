# Hybrid CNN-LSTM Forecasting of SARA-Derived Seismic Amplitude Ratios at Mount Etna

This repository contains the Python implementation used in the study:

**A Hybrid CNN-LSTM Deep Learning Architecture for Network-Scale Forecasting of SARA-Derived Seismic Amplitude Ratios at Mount Etna**

The code implements a hybrid convolutional neural network–long short-term memory (CNN-LSTM) model for forecasting SARA-derived seismic amplitude-ratio time series from the Mount Etna seismic monitoring network. A standalone LSTM model is included as a baseline for comparison.

## Contents

- `stations_LSTM_edit_7(1) (1).ipynb`: Jupyter Notebook containing data preparation, model training, recursive forecasting, and evaluation procedures.

## Requirements

The workflow was developed in Python 3.x using the following packages:

- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Installation

Install the required Python packages:

```bash
pip install tensorflow keras numpy pandas matplotlib scikit-learn jupyter
```

## Data availability

The seismic waveform data used to derive the SARA time series were obtained from the Mount Etna monitoring network operated by the Istituto Nazionale di Geofisica e Vulcanologia (INGV). The original waveform data are not redistributed in this repository. Users should obtain the required data through the relevant INGV data services.

## Quick test

The notebook includes the workflow for model construction, training, forecasting, and evaluation. To run it:

```bash
jupyter notebook "stations_LSTM_edit_7(1) (1).ipynb"
```

Before running the full workflow, users must update the data-file paths and provide the required SARA-derived input time series in the expected format.

## Output

The workflow produces forecasts of SARA-derived seismic amplitude ratios and evaluates the standalone LSTM and hybrid CNN-LSTM models using MSE, RMSE, MAE, and R2.

## License

This repository is released under the MIT License.

## Contact

Ghazaleh Rasaneh  
Email: Gh.Rasaneh@iau.ac.ir
