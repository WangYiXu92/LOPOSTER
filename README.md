# LOPOSTER
Thank you very much for your interest in LOPOSTER, LOBSTER's postprocessor.

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

I have also provided three examples, in accordance with the examples provided in the paper:

Wang, Y.; Mueller, P. C.; Hemker, D.; Dronskowski, R. LOPOSTER: A Cascading Postprocessor for LOBSTER. Journal of Computational Chemistry 2025, 46 (17), e70167. https://doi.org/10.1002/jcc.70167.

In cases of kspace calculations, LOPOSTER can also help to prepare for the NSCF calculation (Please refer to LOBSTER's user manual for more details) by providing an argument: kspace
The command is
```
/path/to/LOPOSTER kspace
```

After the NSCF calculation, one needs to call LOPOSTER again (this time without any argument) for postprocessing.

If you find any bugs or malfunctions, please feel free to reach out to me and I will try my best to fix the problems ASAP.

