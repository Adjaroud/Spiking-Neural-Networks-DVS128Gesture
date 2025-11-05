# Spiking-Neural-Networks-DVS128Gesture
This project implements and trains a **Spiking Neural Network (SNN)** using the **[SpikingJelly]** framework on the **DVS128 Gesture dataset**, a neuromorphic dataset based on event-driven vision sensors.


## Project Overview

This project shows how to:

- Load and preprocess the **DVS128 Gesture** dataset.
- Build a simple SNN model using **Leaky Integrate-and-Fire (LIF)** neurons.
- Train and evaluate the network for gesture classification.

  ## Model Architecture

```text
Input (2 channels, 128×128, 10 frames)
 ↓
Conv2d(2 → 12) + LIF + AvgPool(2)
 ↓
Conv2d(12 → 32) + LIF + AvgPool(2)
 ↓
Flatten + Linear → 11 gesture classes
```

For my first experiment on 3 epochs the accuracy is 67.01%.
For my second experiment on 5 epochs with adding BatchNorm and Dropout. The accuracy is 75.35%.
