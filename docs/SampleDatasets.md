# Sample Datasets for Perfusion MRI

This page provides links to publicly available contrast-agent based perfusion MRI datasets that can be used for research, development, and validation of analysis methods.

## Overview

Sample datasets are essential resources for:
- Developing and validating new analysis methods
- Benchmarking different software tools
- Reproducing published results
- Training and education
- Harmonizing acquisition and analysis protocols across sites

## Available Datasets

### QIN Breast DCE-MRI Dataset

**Provider**: Cancer Imaging Archive (TCIA), Quantitative Imaging Network (QIN)  
**Access**: [TCIA QIN Breast DCE-MRI](https://wiki.cancerimagingarchive.net/display/Public/QIN+Breast+DCE-MRI)  
**Description**: Multisite, multivendor breast DCE-MRI data with associated clinical data. Includes pre-treatment and early-treatment images for monitoring response to neoadjuvant chemotherapy.

### RIDER Neuro MRI Dataset

**Provider**: Cancer Imaging Archive (TCIA)  
**Access**: [TCIA RIDER Neuro MRI](https://wiki.cancerimagingarchive.net/display/Public/RIDER+Neuro+MRI)  
**Description**: DCE-MRI and DSC-MRI scans of brain tumors with test-retest data for reproducibility assessment.

### SPIE-AAPM-NCI PROSTATEx Challenge

**Provider**: Cancer Imaging Archive (TCIA)  
**Access**: [PROSTATEx](https://wiki.cancerimagingarchive.net/display/Public/SPIE-AAPM-NCI+PROSTATEx+Challenges)  
**Description**: Multiparametric MRI of the prostate including DCE-MRI sequences. Includes expert annotations for lesion classification.

### Perfusion Training Dataset

**Provider**: OSIPI Task Force 4.1  
**Access**: [OSIPI Perfusion Training Dataset](https://github.com/OSIPI/OSIPI_StandardizedDatatsets)  
**Description**: Standardized DCE-MRI and DSC-MRI datasets with known ground truth values, specifically curated for training and educational purposes.

### DCE MRI Phantom Dataset

**Provider**: National Institute of Standards and Technology (NIST)  
**Access**: [NIST Quantitative MRI](https://www.nist.gov/programs-projects/quantitative-mri)  
**Description**: Phantom data for testing and validating DCE-MRI quantification methods with controlled conditions and known T1 values.

### KISSDB (Kantonsspital St. Gallen Brain Dataset)

**Provider**: Kantonsspital St. Gallen, Switzerland  
**Access**: [KISSDB Website](https://www.kispi.uzh.ch/en/research/downloads)  
**Description**: DSC-MRI brain perfusion dataset with manual segmentation of stroke lesions and tissue types.

## Dataset Specifications

| Dataset | Modality | Anatomy | # of Subjects | Field Strength | Temporal Resolution | AIF Available |
|---------|----------|---------|---------------|----------------|---------------------|---------------|
| QIN Breast | DCE-MRI | Breast | 67 | 1.5T, 3T | Variable | Yes (some) |
| RIDER Neuro | DCE/DSC | Brain | 19 | 1.5T, 3T | 5-6s | Yes |
| PROSTATEx | DCE-MRI | Prostate | 204 | 3T | 3.5-5s | No |
| OSIPI Training | DCE/DSC | Various | 20 | 1.5T, 3T | Variable | Yes |
| NIST Phantom | DCE-MRI | Phantom | N/A | 1.5T, 3T | Variable | N/A |
| KISSDB | DSC-MRI | Brain | 151 | 1.5T | 1-2s | Yes |

## How to Use These Datasets

1. **Registration**: Most datasets require user registration and agreement to data use terms
2. **Download**: Follow the provider's instructions for downloading the data
3. **Format conversion**: You may need to convert data to formats compatible with your analysis tools
4. **Documentation**: Review the accompanying documentation for acquisition parameters and other metadata
5. **Citation**: Always cite the dataset in your publications according to the provider's guidelines

## Contributing

If you have a publicly available perfusion MRI dataset that you would like to add to this list, please see our [contribution guidelines](contributionTutorial.md).

## References

1. Kalpathy-Cramer J, et al. Quantitative Imaging Network: Data Sharing and Competitive Algorithm Validation Leveraging The Cancer Imaging Archive. Transl Oncol. 2014;7(1):147-52.
2. Shukla-Dave A, et al. Quantitative Imaging Biomarkers Alliance (QIBA) recommendations for improved precision of DWI and DCE-MRI derived biomarkers in multicenter oncology trials. J Magn Reson Imaging. 2019;49(7):e101-e121.
3. Huang W, et al. Variations of dynamic contrast-enhanced magnetic resonance imaging in evaluation of breast cancer therapy response: a multicenter data analysis challenge. Transl Oncol. 2014;7(1):153-66.