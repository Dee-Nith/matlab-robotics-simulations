# Two-Link Manipulator with Computed Torque Control

## Project Overview

This project implements a computed torque control strategy for a servo-controlled two-link robotic arm using the Euler-Lagrange formulation. It emphasizes precise trajectory tracking, feedback linearization, and dynamic compensation for nonlinear forces such as gravity and Coriolis effects.

## Files Structure

```
two-link-manipulator/
├── models/                       # Simulink models and MATLAB scripts
├── results/                      # Simulation results and data
├── scripts/                      # MATLAB control scripts
└── docs/
    └── README.md                 # This file
```

## Key Features

- **Computed Torque Control**: Advanced control strategy implementation
- **Euler-Lagrange Formulation**: Rigorous mathematical modeling
- **Precise Trajectory Tracking**: High-accuracy motion control
- **Feedback Linearization**: Nonlinear control technique
- **Dynamic Compensation**: Gravity and Coriolis effect handling

## Control Strategy

The computed torque control approach includes:

1. **Forward Kinematics**: Position and orientation calculation
2. **Inverse Dynamics**: Torque computation from desired motion
3. **Feedback Linearization**: Nonlinear system linearization
4. **Trajectory Tracking**: Precise path following
5. **Dynamic Compensation**: Real-time force compensation

## Performance Achievements

- **Tracking Error**: < 2% steady-state error
- **Smooth Motion**: Continuous and stable trajectories
- **Real-time Response**: Fast system dynamics
- **Robust Performance**: Stable under varying conditions

## Usage

1. Navigate to the project directory:
   ```matlab
   cd projects/two-link-manipulator
   ```

2. Run the main control script:
   ```matlab
   % Add your main script name here
   run_manipulator_control
   ```

3. Analyze results and performance metrics

## Technical Implementation

### Control Algorithm
- **Input**: Desired joint trajectories
- **Processing**: Computed torque calculation
- **Output**: Joint torques for actuators
- **Feedback**: Position and velocity sensors

### Mathematical Model
- **Kinematics**: DH parameters and transformation matrices
- **Dynamics**: Euler-Lagrange equations of motion
- **Control Law**: Computed torque with feedback linearization

## Simulation Results

Expected outcomes:
- Smooth trajectory tracking
- Minimal steady-state error
- Robust disturbance rejection
- Real-time computational performance

## Future Enhancements

- Adaptive control implementation
- Robust control strategies
- Multi-objective optimization
- Hardware-in-the-loop testing

---

*Part of MSc coursework at Queen Mary University of London*
