# Analysis Toolboxes for Perfusion MRI

This page provides an overview of software tools and packages designed for the analysis of contrast-agent based perfusion MRI data.

## Overview

Perfusion MRI analysis toolboxes provide implementations of various algorithms for quantifying perfusion parameters from DCE-MRI and DSC-MRI data. These tools facilitate the conversion of signal intensity time courses into quantitative perfusion metrics using pharmacokinetic models and other quantification approaches.

## Available Analysis Toolboxes

### QIN-PROQC (Quantitative Imaging Network - Perfusion Research Oncology Quality Control)

**Developer**: Quantitative Imaging Network (QIN)  
**Repository**: [GitHub Repository](https://github.com/DrSidG/QIN-PROQC)  
**Description**: A MATLAB-based platform for quality control and standardization of DCE-MRI analysis in oncology. It includes implementations of several tracer kinetic models including Tofts, Extended Tofts, and Patlak.

### ROCKETSHIP

**Developer**: Stanford University  
**Repository**: [GitHub Repository](https://github.com/petmri/ROCKETSHIP)  
**Description**: A MATLAB-based toolkit for kinetic modeling of DCE-MRI data. It provides a comprehensive workflow from T1 mapping to parametric map generation.

### PkModeling

**Developer**: Quantitative Image Informatics for Cancer Research (QIICR)  
**Repository**: [GitHub Repository](https://github.com/QIICR/PkModeling)  
**Description**: A C++ library for pharmacokinetic analysis of DCE-MRI, integrated with 3D Slicer via the PkModeling extension.

### DCE-MRI.jl

**Developer**: Julia MRI community  
**Repository**: [GitHub Repository](https://github.com/notZaki/DCE-MRI.jl)  
**Description**: A Julia package for DCE-MRI analysis with implementations of various pharmacokinetic models and AIF estimation methods.

### DCE-Tool

**Developer**: Danish Research Centre for Magnetic Resonance  
**Website**: [DCE-Tool Website](https://www.drcmr.dk/software)  
**Description**: A MATLAB-based tool for DCE-MRI analysis with a graphical user interface, supporting multiple pharmacokinetic models.

### DSCoMAN (DSC-MRI Analysis)

**Developer**: Medical College of Wisconsin  
**Website**: [DSCoMAN Website](https://mcw.edu/departments/biophysics/research/software)  
**Description**: A software package for the analysis of DSC-MRI data, providing relative and absolute cerebral blood flow, blood volume, and mean transit time maps.

### Perfusion BASIL

**Developer**: FMRIB Centre, University of Oxford  
**Website**: [BASIL Website](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/BASIL)  
**Description**: Although primarily designed for arterial spin labeling, BASIL includes tools that can be adapted for contrast-based perfusion analysis.

## Comparison of Key Features

| Toolbox | Platform | Models Supported | GUI | AIF | Open Source |
|---------|----------|------------------|-----|-----|-------------|
| QIN-PROQC | MATLAB | Tofts, ETM, Patlak | Yes | Manual, Auto | Yes |
| ROCKETSHIP | MATLAB | Tofts, ETM, 2CXM | Yes | Manual, Auto | Yes |
| PkModeling | C++/3D Slicer | Tofts, ETM | Yes | Manual | Yes |
| DCE-MRI.jl | Julia | Tofts, ETM, 2CXM | No | Manual, Auto | Yes |
| DCE-Tool | MATLAB | Tofts, ETM, 2CXM | Yes | Manual | Yes |
| DSCoMAN | MATLAB | SVD, cSVD | Yes | Auto | Yes |
| BASIL | C++/FSL | Kinetic models | Yes | N/A | Yes |

## How to Select an Analysis Toolbox

Consider the following factors when selecting a toolbox for your perfusion MRI analysis:

1. **Compatibility**: Ensure the toolbox works with your data format and operating system
2. **Models implemented**: Check if the toolbox includes the pharmacokinetic models you need
3. **Validation**: Look for toolboxes that have been validated in published literature
4. **Support and documentation**: Consider the availability of documentation and user support
5. **Customizability**: Determine if you need to modify or extend the existing analysis methods

## Contributing

If you have developed an analysis toolbox for contrast-agent based perfusion MRI that you would like to add to this list, please see our [contribution guidelines](contributionTutorial.md).

## References

1. Sourbron SP, Buckley DL. Tracer kinetic modelling in MRI: estimating perfusion and capillary permeability. Phys Med Biol. 2012;57(2):R1-33.
2. Heye AK, et al. Assessment of blood-brain barrier disruption using dynamic contrast-enhanced MRI. A systematic review. NeuroImage Clin. 2014;6:262-74.
3. Jahng GH, et al. Perfusion magnetic resonance imaging: a comprehensive update on principles and techniques. Korean J Radiol. 2014;15(5):554-77.