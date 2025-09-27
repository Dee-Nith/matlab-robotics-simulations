# Rotating Arm Mechanism Simulation

## Project Overview

This project simulates a rotating arm mechanism with oscillatory motion using MATLAB Simulink and Mechanics Explorer. It demonstrates rigid body dynamics, harmonic motion, and matrix operations in a simulated environment.

## Files Structure

```
rotating-arm/
├── models/
│   ├── Main_System.slx           # Main Simulink model
│   └── Main_System.slx.original  # Original backup
├── results/
│   └── Results.xlsx              # Simulation results and metrics
├── scripts/                      # MATLAB analysis scripts (to be added)
└── docs/
    └── README.md                 # This file
```

## Key Features

- **Rigid Body Dynamics**: Accurate modeling of mechanical systems
- **Harmonic Motion**: Oscillatory behavior simulation
- **Matrix Operations**: Advanced mathematical computations
- **Real-time Visualization**: Mechanics Explorer integration

## Performance Metrics

- **Error Margins**: < 2% tracking error
- **Response Time**: Real-time system response
- **Stability**: Robust performance under dynamic conditions

## Usage

1. Open MATLAB and navigate to this directory
2. Open the Simulink model:
   ```matlab
   open('models/Main_System.slx')
   ```
3. Run the simulation and analyze results in `Results.xlsx`

## Technical Details

- **Solver**: ode45 (default)
- **Simulation Time**: Configurable
- **Output**: Position, velocity, and acceleration data
- **Visualization**: 3D mechanics explorer

## Results Analysis

Check `results/Results.xlsx` for:
- Trajectory tracking performance
- Error analysis
- System response characteristics
- Performance metrics

---

*Part of MSc coursework at Queen Mary University of London*
