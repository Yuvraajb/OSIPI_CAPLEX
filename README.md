# The contrast-agent based perfusion lexicon (CAPLEX)  [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8180201.svg)](https://doi.org/10.5281/zenodo.8180201)

## Overview 

The ISMRM Open Science Initiative for Perfusion Imaging (OSIPI) aims to promote the sharing of perfusion imaging software in order to reduce duplication, improve reproducibility and speed up translation. This repository contains the github pages content for the lastest version of the contrast agent based perfusion lexicon. 

The lexicon was developed and maintained by Taskforce 4.2 of OSIPI and aims to define standadised terminology and definitions for commonly used quantities, models, and processes used in DCE-MRI and DSC-MRI analyses. 

The lexicon is hosted as a github page website (osipi.github.io/OSIPI_CAPLEX/). 

## Repository contents
The repo is in development but currently contains:

1. the "editable" markdown (.md) files that define the webpage content (in the **/docs** directory).
2. the "non-editable" backend for the CAPLEX webpage generated when .md files on main are deployed (found on the **gh-pages** branch)
3. XML schema files (under development!!!) and examples for lexicon-linked algorithmic encoding (in the **/Algorithmic-encoding** directory)

## Adding lexicon hyperlinks to your methods/results text (lexicon-linked free text format)
We recommend that lexicon terminology is used in all DCE\DSC manuscripts and documentation to reduce variability in reporting. We also recommend that individual references to lexicon entries are linked directly to the webpage entry for that entry using a hyperlink. We are working on developing a tool that makes this process easier, but for the time-being these entries need to be added manually. The following steps need to be taken:

1. Find the **a code**. Go to the relevant .md file for on **/docs** directory of main (e.g. quantities.md). Either open the file on github (and select *Code* tab) or open in your local repo in a text editor. Search for the entry of interest and find the ```<a name="..."></a>``` snippet for the entry of interest. This can be found in the OSIPI name column. An example is given below:

```
| Q.MS1.001.[j] | <a name="S"></a> Signal | -- | *S<sub>j</sub>* | The MR signal (magnitude, phase or complex depending on context) in compartment *j*. | a.u. | -- |
```

2. Make the hyperlink. The part of ```<a name="..."></a>``` in quotation marks must be added to the webpage name as follows: osipi.github.io/OSIPI_CAPLEX/*add section name here*/# *add part in quotation marks here*.  

In this example, the **a code** is *S* and the section name is *quantities*. So the full hyperlink is  osipi.github.io/OSIPI_CAPLEX/quantities/#S. A # symbol must be added immediately after the slash and prior to the **a code**.

Once you have constructed the hyperlink, test it works by entering the address in your browser. The link should take you directly to the quantity, process or model being referenced. 

3. Add the hyperlink to the relevant entry in your manuscript or documentation.

## Contributing to the lexicon
The lexicon is designed to the extensible and we actively engage researchers in the DCE/DSC MRI field to engage with its usage and development. If you would like to add or edit content (new entries etc.) of the lexicon, please either:
1. contact the task force leads (currently Ben Dickie (ben.dickie@manchester.ac.uk)) with your proposed changes. These will be reviewed at the next Task Force meeting (usually monthly).
2. OR create a development branch of main and edit the .md files directly. Once done, submit a pull request (do not merge with main!), which will then be reviewed by the Task Force.     

## Suggesting edits or additions to lexicon entries

Edits or altogether new entries can be suggested by editing the .md files found within the **/docs** directory. To do this, make a new *development* branch of main and edit the .md files as necessary. Some basic instructions on how to edit markdown files are given here: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

Below is an excerpt from the quantities.md file:

```
## <a name="Electromagnetic quantities"></a> Electromagnetic quantities
The items in this group are related to electromagnetic tissue properties and electromagnetic properties of contrast agents. The abbreviations SE and GE denote spin and gradient echo.

 | Code | OSIPI name| Alternative names|Notation|Description|OSIPI units|Reference|
 | -- | -- | -- | -- | -- | -- | -- |
 | Q.EL1.001.[j]| <a name="R1"></a> Longitudinal relaxation rate | *R<sub>1</sub>* -relaxation rate | *R<sub>1,j</sub>* | Longitudinal relaxation rate in compartment *j*. | 1/s | -- |
 | Q.EL1.002.[j] | <a name="R10"></a> Native longitudinal relaxation rate |Baseline *R<sub>1</sub>* | *R<sub>10,j</sub>* | Longitudinal relaxation rate in compartment *j*. | 1/s | -- |
 ...
 | Q.EL1.019 | <a name="r1b"></a> Longitudinal relaxivity of bound indicator | -- | *r<sub>1,b</sub>*  | Longitudinal relaxivity of bound indicator. | 1/s/mM | -- |
 | Q.EL1.020 | <a name="k1k2"></a> Transverse relaxivities of the quadratic model (GE) | -- | [*k<sub>1</sub>*,k<sub>2</sub>] | First and second order relaxivities for the quadratic model of the transverse relaxation rate (GE) | [1/s/mM,1/s/mM]| -- |
 | Q.EL1.999 | <a name="not listed EL1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |
```

To add a new entry, identify the section and group that makes the most sense, then simply add a new line to the .md file between the last numbered entry and the **not listed** entry. Remember to assign a new code (usually the same as the previous entry but incremented by 1).

For example:

```
| Q.EL1.020 | <a name="k1k2"></a> Transverse relaxivities of the quadratic model (GE) | -- | [*k<sub>1</sub>*,k<sub>2</sub>] | First and second order relaxivities for the quadratic model of the transverse relaxation rate (GE) | [1/s/mM,1/s/mM]| -- |
| Q.EL1.021 | <a name="new link"></a> New quantity                                    | **add alternative name here** | **add notation here** | **add description here** | **add units here** | **add reference here** |
| Q.EL1.999 | <a name="not listed EL1"></a> Quantity not listed | -- | -- | This is a custom free-text item, which can be used if a quantity of interest is not listed. Please state a literature reference and request the item to be added to the lexicon for future usage. | [variable] | -- |
```

Once done, commit the changes and submit a pull request. Make sure to add a description of the changes when making the pull request. 

## Deploying changes
After careful review, proposed changes to markdown files made on a development branch will be merged into the *main* branch. After the merge is approved, this will trigger a CI workflow to automatically generate the new docs and publish to the *gh-pages* branch, **which should not be edited manually**.

