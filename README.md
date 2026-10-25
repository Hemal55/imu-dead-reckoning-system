# IMU-Based Dead Reckoning System

A deep-learning project for vehicle speed prediction from inertial measurement unit (IMU) sensor data and 2D trajectory reconstruction.

## Overview

This project explores the use of sequential sensor data and recurrent neural networks to estimate vehicle speed and reconstruct a vehicle's trajectory.

## Key Features

- **Speed prediction:** A Convolutional Recurrent Neural Network (CRNN) combining 1D convolutional layers and a two-layer GRU.
- **Sensor processing:** Gravity compensation and feature scaling for IMU data.
- **Trajectory reconstruction:** Uses predicted speed and gyroscope-derived heading to reconstruct a 2D path.
- **Model evaluation:** Compares reconstructed trajectories against a reference path and a conventional double-integration baseline.
- **Visualisation:** Generates plots for trajectory comparison and prediction analysis.

## Technologies

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib

## Project Structure

The repository includes scripts for model training, data generation, testing, error calculation, trajectory mapping, and visualisation.

## Results

The project includes plots and evaluation scripts for analysing speed predictions and trajectory reconstruction. Refer to the included visualisations for the comparisons produced by the current implementation.

## Future Improvements

- Evaluate performance on additional independent driving datasets.
- Improve trajectory estimation and reduce accumulated position error.
- Document reproducible training and evaluation procedures.

## Disclaimer

This is an experimental project. Trajectory reconstruction accuracy depends on sensor quality, model performance, and accumulated estimation error.
