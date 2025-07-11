# LOPOSTER
Thank you very much for your interest in LOPOSTER, LOBSTER's postprocessor.
![TOC](https://github.com/user-attachments/assets/3ff770df-4a9a-4caa-9298-78bb4ad27001)


## Features
- Generation of lobsterin files for real space and kspace analyses
- Automatic handling of datafiles from LOBSTER (e.g. COHPCAR.lobster, ICOHPLIST.lobster......)
- Automatic handling of a mixture of two-center and multicenter COBI.
- Automatic calculation and visualization of on-site and off-site cumulative COHP
- Automatic visualization of orbital contribution matrix of a chemical bond
- Automatic handling of results with spin polarization
- Automatic plotting of IMOFE matrix
- Automatic plotting of fatband and kspace COHP data
- Parallelization supported for enhanced efficiency
- Binary files available, no installation needed

## Download
For Linux users: Please download `loposter`

For Windows users: Please download `loposter.exe`

## Usage
To use the software, one simply needs to download the corresponding executable file that can be run on your computer.

One can simply invoke the program by:

For Linux:
```
/path/to/LOPOSTER
```
For Windows:
```
Please double click the icon
```
Or one simply repeats the way to call LOBSTER (You know how to use LOBSTER, don't you?)

## Examples

I have also provided three examples, in accordance with the examples provided in the paper:

Wang, Y.; Mueller, P. C.; Hemker, D.; Dronskowski, R. LOPOSTER: A Cascading Postprocessor for LOBSTER. Journal of Computational Chemistry 2025, 46 (17), e70167. https://doi.org/10.1002/jcc.70167.

|Name|Explanation|
|---|---|
|Example_1|NiNCN without spin polarization|
|Example_2|NiNCN with spin polarization and FM initial configuration|
|Example_3|NiNCN with spin polarization and AFM initial configuration|

## Citation

We kindly request that users of LOPOSTER cite the following paper:

In ACS format:
Wang, Y.; Mueller, P. C.; Hemker, D.; Dronskowski, R. LOPOSTER: A Cascading Postprocessor for LOBSTER. Journal of Computational Chemistry 2025, 46 (17), e70167. https://doi.org/10.1002/jcc.70167.

In BibTex format:
```
@article{https://doi.org/10.1002/jcc.70167,
author = {Wang, YiXu and M{\"u}ller, Peter C. and Hemker, David and Dronskowski, Richard},
title = {LOPOSTER: A Cascading Postprocessor for LOBSTER},
journal = {Journal of Computational Chemistry},
volume = {46},
number = {17},
pages = {e70167},
keywords = {carbodiimide, chemical bonding, LOBSTER, magnetic ordering, postprocessing},
doi = {https://doi.org/10.1002/jcc.70167},
url = {https://onlinelibrary.wiley.com/doi/abs/10.1002/jcc.70167},
eprint = {https://onlinelibrary.wiley.com/doi/pdf/10.1002/jcc.70167},
note = {e70167 3504320},
abstract = {ABSTRACT The computer program LOPOSTER, available via GitHub, is introduced, capable of postprocessing the LOBSTER code results. LOPOSTER is designed to be particularly effective for analyzing large datasets with over 10,000 interactions and enormously reducing postprocessing time. LOPOSTER pioneers the automated processing of advanced bonding analysis results, including multicenter bonding, molecular-orbital formation energy, and k-dependent COHP, expanding the scope of routine chemical-bonding investigations. In addition, LOPOSTER streamlines the postprocessing workflow by providing comprehensive results in a single execution, minimizing user intervention and potential errors. An example of chemical-bonding analysis on NiNCN is provided, with visualization by LOPOSTER. LOPOSTER offers versatile analysis of interactions in NiNCN, enabling evaluations in real or reciprocal space, and based on atomic or molecular orbitals, catering to different analytic preferences. Various correlations between those interactions and magnetism in NiNCN are also explored. The electron-rich features of an N=C=N π bond have been discussed from various perspectives.},
year = {2025}
}
```

## Preparing for kspace calculations
In cases of kspace calculations, LOPOSTER can also help to prepare for the NSCF calculation (Please refer to LOBSTER's user manual for more details) by providing an argument: kspace
The commands are:

For Linux:
```
/path/to/LOPOSTER kspace
```
For Windows (NOT subsystem):
```
\path\to\LOPOSTER.exe kspace
```

After the NSCF calculation, one needs to call LOPOSTER again (this time without any argument) for postprocessing.

If you find any bugs or malfunctions, please feel free to reach out to me and I will try my best to fix the problems ASAP.

## Control the x axis
To control the x axis, one needs to add the following line in the `lobsterin` file:
`!xrange x_min x_max`
Please note that the `!` is necessary and will help you to refrain from disturbing LOBSTER run.


