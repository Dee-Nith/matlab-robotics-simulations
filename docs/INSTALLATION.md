# Installation Guide

This guide will help you set up the MATLAB Robotics Simulations environment on your system.

## 📋 Prerequisites

### System Requirements
- **Operating System**: Windows 10/11, macOS 10.15+, or Linux (Ubuntu 18.04+)
- **RAM**: Minimum 8GB (16GB recommended)
- **Storage**: At least 2GB free space
- **Processor**: Multi-core processor (Intel i5/AMD Ryzen 5 or better)

### Software Requirements
- **MATLAB R2023a** or later
- **Simulink** (included with MATLAB)
- **Control System Toolbox** (recommended)
- **Robotics System Toolbox** (recommended)
- **Symbolic Math Toolbox** (for advanced calculations)

## 🚀 Installation Steps

### 1. Install MATLAB

#### Option A: Academic License (Recommended)
1. Visit [MathWorks Academic](https://www.mathworks.com/academia/)
2. Download MATLAB with your university credentials
3. Follow the installation wizard
4. Activate with your academic license

#### Option B: Trial Version
1. Visit [MathWorks Trial](https://www.mathworks.com/products/matlab/trial.html)
2. Download the 30-day trial
3. Complete the installation process

### 2. Install Required Toolboxes

After MATLAB installation, install the recommended toolboxes:

```matlab
% Open MATLAB and run:
matlab.addons.install('Control System Toolbox')
matlab.addons.install('Robotics System Toolbox')
matlab.addons.install('Symbolic Math Toolbox')
```

### 3. Clone the Repository

```bash
# Using Git
git clone https://github.com/yourusername/matlab-robotics-simulations.git
cd matlab-robotics-simulations

# Or download as ZIP and extract
```

### 4. Set Up MATLAB Path

Add the project directories to your MATLAB path:

```matlab
% In MATLAB command window:
addpath(genpath('projects/two-link-manipulator'))
addpath(genpath('projects/rotating-arm'))
addpath(genpath('assets'))
```

### 5. Verify Installation

Run the verification script:

```matlab
% Check MATLAB version
version

% Check available toolboxes
ver

% Test basic functionality
cd projects/rotating-arm
open('models/Main_System.slx')
```

## 🔧 Configuration

### MATLAB Preferences
1. **Set working directory** to the project root
2. **Configure Simulink preferences**:
   - Solver: ode45 (default)
   - Max step size: auto
   - Relative tolerance: 1e-3

### Performance Optimization
For better simulation performance:

```matlab
% Set MATLAB to use multiple cores
maxNumCompThreads('automatic')

% Optimize Simulink for speed
set_param(0, 'SimulationMode', 'accelerator')
```

## 🧪 Testing the Installation

### Test 1: Two-Link Manipulator
```matlab
cd projects/two-link-manipulator
% Run your control scripts here
fprintf('Two-link manipulator project ready!\n')
```

### Test 2: Rotating Arm Mechanism
```matlab
cd projects/rotating-arm
open('models/Main_System.slx')
% The Simulink model should open without errors
fprintf('Rotating arm mechanism ready!\n')
```

## 🐛 Troubleshooting

### Common Issues

#### MATLAB License Error
```
Error: License checkout failed
```
**Solution**: Verify your license is active and has the required toolboxes.

#### Simulink Model Won't Open
```
Error: Cannot open model file
```
**Solution**: Ensure you have Simulink installed and the file path is correct.

#### Performance Issues
**Symptoms**: Slow simulation, high memory usage
**Solutions**:
- Close unnecessary MATLAB windows
- Use accelerator mode in Simulink
- Increase system RAM if possible

### Getting Help

1. **Check MATLAB Documentation**: `doc` command in MATLAB
2. **MathWorks Support**: [Support Center](https://www.mathworks.com/support/)
3. **Community Forums**: [MATLAB Central](https://www.mathworks.com/matlabcentral/)
4. **Project Issues**: Create an issue in this repository

## 📚 Additional Resources

### Learning MATLAB
- [MATLAB Onramp](https://matlabacademy.mathworks.com/) - Free interactive tutorial
- [Simulink Onramp](https://matlabacademy.mathworks.com/) - Simulink basics
- [Control Systems Onramp](https://matlabacademy.mathworks.com/) - Control theory

### Robotics Resources
- [Robotics System Toolbox Documentation](https://www.mathworks.com/help/robotics/)
- [Peter Corke's Robotics Toolbox](https://petercorke.github.io/robotics-toolbox-matlab/)

## ✅ Installation Checklist

- [ ] MATLAB R2023a+ installed and activated
- [ ] Simulink available and working
- [ ] Required toolboxes installed
- [ ] Repository cloned/downloaded
- [ ] MATLAB path configured
- [ ] Test simulations running successfully
- [ ] Performance optimized (optional)

## 🆘 Support

If you encounter issues during installation:

1. Check this troubleshooting guide
2. Search existing issues in the repository
3. Create a new issue with detailed information
4. Contact the repository maintainer

---

*Happy simulating! 🚀*
