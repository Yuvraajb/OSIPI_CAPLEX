# Data Simulation Tools for Perfusion MRI

This page provides an overview of software tools for simulating contrast-agent based perfusion MRI data, which can be valuable for testing and validating perfusion quantification methods.

## Overview

Simulation tools allow researchers to generate synthetic perfusion MRI data with known ground truth parameters. These tools are essential for:

- Validating quantification algorithms
- Testing the effects of noise, temporal resolution, and other acquisition parameters
- Developing and benchmarking new analysis methods
- Training and education

## Available Simulation Tools

### JSim

**Developer**: University of Washington, Physiome Project  
**Website**: [JSim Website](http://www.physiome.org/jsim/)  
**Description**: JSim is a Java-based simulation system for building quantitative numerical models and analyzing them with respect to experimental reference data. It can be used to simulate tracer-kinetic models for DCE-MRI and DSC-MRI.

### OSIPI DCE/DSC Simulator

**Developer**: OSIPI Task Force 1.2  
**Repository**: [GitHub Repository](https://github.com/OSIPI/TF1.2_notebook)  
**Description**: A collection of Jupyter notebooks developed by OSIPI for simulating DCE-MRI and DSC-MRI data with various perfusion models. These notebooks allow users to generate synthetic perfusion time-series with user-defined parameter values.

### POSSUM (Physics-Oriented Simulated Scanner for Understanding MRI)

**Developer**: FMRIB Centre, University of Oxford  
**Website**: [POSSUM Website](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/POSSUM)  
**Description**: Although primarily designed for fMRI, POSSUM can be adapted for simulating perfusion MRI with the addition of tracer-kinetic models.

### JEMRIS (Jülich Extensible MRI Simulator)

**Developer**: Forschungszentrum Jülich  
**Website**: [JEMRIS Website](http://www.jemris.org/)  
**Description**: JEMRIS is an open-source MRI simulator that includes capabilities for simulating various pulse sequences and can be extended to include contrast agent dynamics.

## How to Use Simulation Tools in Perfusion Research

1. **Define physiological parameters**: Set tissue-specific parameters (e.g., blood flow, vessel permeability, blood volume) based on literature or experimental values.
2. **Set up acquisition parameters**: Configure temporal resolution, noise level, and other MRI acquisition parameters.
3. **Run simulation**: Generate synthetic perfusion time-series data.
4. **Apply analysis methods**: Test different quantification methods on the simulated data.
5. **Compare results with ground truth**: Evaluate the accuracy of quantification methods.

## Contributing New Simulation Tools

If you have developed a simulation tool for contrast-agent based perfusion MRI that you would like to add to this list, please see our [contribution guidelines](contributionTutorial.md).

## References

1. Jelescu IO, et al. Challenges for biophysical modeling of microstructure. J Neurosci Methods. 2020;344:108861.
2. Sourbron SP, Buckley DL. Classic models for dynamic contrast-enhanced MRI. NMR Biomed. 2013;26(8):1004-27.
3. Koh TS, et al. Fundamentals of tracer kinetics for dynamic contrast-enhanced MRI. J Magn Reson Imaging. 2011;34(6):1262-76.