# position-specific-kie


## Getting started
To clone the remote repository to your local drive and create a new directory on your local drive and at the same time:

- Go to the parent directory where you want to put this repository:
```
cd parent_directory
```

- Clone this remote repo into a new sub-directory and navigate to that sub-directory.
	- For GitHub (non-GLBRC) users:
```
git clone https://github.com/GLBRC/position-specific-KIE
cd new_sub_directory
```

	- For GLBRC users:
```
git clone https://gitpub.wei.wisc.edu/rivettel/position-specific-kie.git
cd new_sub_directory
```

In this example, the new sub-directory is named "new_sub_directory".

You can now run the markdown (.qmd) files in the `code` sub-directory using Rstudio.

Cloning the repository to your local drive also created empty sub-directories under `ouput` that will be populated if you run the code in the markdown file with the corresponding name.
To write files properly, the package `here` has to be loaded in the `expanded_ray` sub-directory.


## Sub-directories in this repository
`code` contains multiple markdown files (.qmd) with code that can be run in R. Each file is dedicated to analysis of a specific dataset.

- delta_so_limits_oub.qmd
	- Table S1- Absolute relative error of εN-bulk and KIE values introduced by Mariotti’s approximation of the Rayleigh equation at various δ15Ns0 values
	- Table S2. Absolute relative error of εN-bulk and KIE values introduced by varying εN-bulk values

- exp_hydroxylamine_ox_pub.qmd - Code for analyzing previously published data on hydroxylamine oxidation (Sutka et al., 2006)
	- Figure 4. Experimentally measured δ15N values for N2O synthesis from NH2OH in a pure culture of Methylosinus trichosporium (data from (Sutka et al., 2006)).
	- Table 5. Comparison of standard Rayleigh and Expanded Rayleigh KIE values ± standard error for N2O produced from NH2OH by an axenic culture of M. trichosporium (Methylocystis sp.). Values were calculated using isotopic data previously published for M. trichosporium replicate B (Sutka et al., 2006)].
	- Table S14. N2O concentrations and δ15Nbulk values (reported) and values of δ15Nα, δ15Nβ (back-calculated) for N2O production from NH2OH by M. trichosporium replicate B [isotopic data previously published (Sutka et al., 2006)].
	- Table S15. Comparison of values calculated for the standard and Expanded Rayleigh models for N2O production from NH2OH by an axenic culture of M. trichosporium (Methylocystis sp.).

- Exp_P450_NOR_pub.qmd - Code for analyzing previously published data on P450-NOR catalyzed reduction of NO to N2O (Yang et al., 2014)
	- Figure 5. Experimentally measured product δ15N values and calculated δ15Ns0 values for N2O synthesis from NO by purified H. capsulatum P450 NOR (data from (Yang et al., 2014)).
	- Table 6. Comparison of standard Rayleigh and Expanded Rayleigh KIE values ± standard error for N2O production from NO by purified Histoplasma capsulatum (fungal) P450 NOR [calculated using previously published isotopic data (Yang et al., 2014)].
	- Table S16. N2O concentrations and product δ values (δ15Nbulk, δ15Nα, and δ15Nβ) reported for N2O production from NO by purified Histoplasma capsulatum (fungal) P450 NOR [isotopic data previously published (Yang et al., 2014)].
	- Table S17. Comparison of values calculated for the standard and Expanded Rayleigh models for N2O production from NO by purified Histoplasma capsulatum (fungal) P450 NOR [calculated using previously published isotopic data (Yang et al., 2014)].

- sim1_no_KIE_normal_KIE_pub.qmd - Code for simulating Dataset 1: No KIE 15Nα, Normal KIE 15Nβ
	- Figure 3. Example simulations derived from Dataset 1 with varying levels of error and types of skewness.
	- Figure 6. Dataset 1: Comparison of the accuracy and goodness of fit of the standard Rayleigh model and Expanded Rayleigh models 1 and 2.
	- Table S4. Dataset 1: Simulated no-error values for N2O synthesis in a closed system (no isotope effect for Nα, normal isotope effect for Nβ).
	- Table S9. Precision and accuracy of values calculated with the Expanded Rayleigh model using simulated datasets derived from Dataset 1 (no isotope effect for Nα, normal isotope effect for Nβ).

- sim1-sim5_v3.qmd - Code for generating error-free simulated Datasets 1-5
	- Figure 1. Simulated δ15N values for N2O synthesis in a closed system with different combinations of KIE 15Nα and KIE 15Nβ.

- sim2_normal_KIEs_pub.qmd - Code for simulating Dataset 2: Normal KIE 15Nα, Normal KIE 15Nβ
	- Figure S1. Example datasets derived from Dataset 2 with varying levels of error and types of skewness.
	- Figure S5. Dataset 2: Comparison of the accuracy and goodness of fit of the standard Rayleigh model and Expanded Rayleigh models 1 and 2.
	- Table S5. Dataset 2: Simulated no-error values for N2O synthesis in a closed system (normal isotope effect for Nα, normal isotope effect for Nβ).
	- Table S10. Precision and accuracy of values calculated with the Expanded Rayleigh model using simulated datasets derived from Dataset 2 (normal isotope effects for Nα and Nβ).

- sim3_inverse_normal_KIEs_pub.qmd - Code for simulating Dataset 3: Inverse KIE 15Nα, Normal KIE 15Nβ
	- Figure S2. Example datasets derived from Dataset 3 with varying levels of error and types of skewness.
	- Figure S6. Dataset 3: Comparison of the accuracy and goodness of fit of the standard Rayleigh model and Expanded Rayleigh models 1 and 2.
	- Table S6. Dataset 3: Simulated no-error values for N2O synthesis in a closed system (inverse isotope effect for Nα, normal isotope effect for Nβ).
	- Table S11. Precision and accuracy of values calculated with the Expanded Rayleigh model using simulated datasets derived from Dataset 3 (inverse isotope effect for Nα, normal isotope effect for Nβ).

- sim4_inverse_KIEs_pub.qmd - Code for simulating Dataset 4: Inverse KIE 15Nα, Inverse KIE 15Nβ
	- Figure S3. Example datasets derived from Dataset 4 with varying levels of error and types of skewness.
	- Figure S7.  Dataset 4: Comparison of the accuracy and goodness of fit of the standard Rayleigh model and Expanded Rayleigh models 1 and 2.
	- Table S7. Dataset 4: Simulated no-error values for N2O synthesis in a closed system (inverse isotope effect for Nα, inverse isotope effect for Nβ).
	- Table S12. Precision and accuracy of values calculated with the Expanded Rayleigh model using simulated datasets derived from Dataset 4 (inverse isotope effects for Nα and Nβ).

- sim5_normal_KIE_no_KIE_pub.qmd - Code for simulating Dataset 5: Normal KIE 15Nα, No KIE 15Nβ
	- Figure S4. Example datasets derived from Dataset 5 with varying levels of error and types of skewness.
	- Figure S8. Dataset 5: Comparison of the accuracy and goodness of fit of the standard Rayleigh model and Expanded Rayleigh models 1 and 2.
	- Table S8. Dataset 5: Simulated no-error values for N2O synthesis in a closed system (normal isotope effect for Nα, no isotope effect for Nβ).
	- Table S13. Precision and accuracy of values calculated with the Expanded Rayleigh model using simulated datasets derived from Dataset 5 (normal isotope effects for Nα, no isotope effect for Nβ).

- tau_limit_pub
	- Table S3. Testing the impact of ρ and τ values on the Expanded Rayleigh model

`data` has two sub-directories: `input` and `output`.
- `input` contains .csv files needed for analyzing previously published experimental data (hydroxylamine oxidation by pure cultures, NO reduction by fungal P450 NOR).
- `output` has a sub-directory for each markdown file where the final .csv files will be stored.
For example, output for `sim1.qmd` will be stored at "your_local_directory\position-specific-kie\data\output\sim1".

`graphs` has a sub-directory for each markdown file where graphs are stored (as .tiff or .png files). This includes the plots used to make the figures shown in the paper (main text and SI).

	
## General outline for analyzing experimental data:
- Load packages
- Load data
	- Table S14, Table S16
- Calculate additional values needed for analysis
	- Table S14
- Apply standard Rayleigh model
	- Plot histogram of residuls for bulk N linear regression
	- Figures 4-5: Plot δ15N vs (1-f)
	- Plot δ15N vs [-flnf/(1-f)]
- Apply Expanded Rayleigh model
- Combine results in summary table(s)
	- Tables 5-6, Table S15, Table S17

## General outline for analyzing simulated data:
- Load packages
- Simulate error-free dataset
	- Plot δ15N values vs (1-f)
	- Tables S4-S8: Simulated no-error values for Datasets 1-5

- Analysis of single datasets (no-error dataset and one example for each combination of error level and skewness (e1-e9))
	- Generate simulated dataset w/ appropriate error/skewness
		- Plot δ15N values vs (1-f)
		- Plot δ15N values vs [-flnf/(1-f)]
	- Apply standard Rayleigh model
		- Assess distriubtion of residuls for bulk N linear regression and plot histogram
	- Apply Expanded Rayleigh model (nonlinear models 1 and 2)
		- Assess distriubtion of residuls for bulk N nonlinear regression and plot histogram
	- Make a summary table for each individual dataset
- Combine results of the analyses of single datasets
	- Make summary table
	- Figure 3, Figures S1-S4: Plot δ15N values vs (1-f)
	- Figure 6, Figures S5-S8: Bar graphs comparing accuracy (KIE values) and goodness of fit (RMSE) for the standard and Expanded Rayleigh models (1 and 2)  

- Analysis of 1000 simulated datasets at each combination of error level and skewness (e1-e9)
	- 
	-Tables S9-S13: Precision and accuracy of Expanded Rayleigh model 1 and 2 values for Datasets 1-5


## Authors
Elise Rivett

## References
Hayes, J. M.: An introduction to isotopic calculations, Woods Hole Oceanographic Institution, Woods Hole, MA 02543, USA, 2004.

Mariotti, A., Germon, J. C., Hubert, P., Kaiser, P., Letolle, R., Tardieux, A., and Tardieux, P.: Experimental determination of nitrogen kinetic isotope fractionation: Some principles; illustration for the denitrification and nitrification processes, Plant Soil, 62, 413-430, 10.1007/BF02374138, 1981.

Sutka RL, Ostrom NE, Ostrom PH, Breznak JA, Gandhi H, Pitt AJ, Li F. Distinguishing nitrous oxide production from nitrification and denitrification on the basis of isotopomer abundances. Appl Environ Microbiol. 2006 Jan;72(1):638-44. doi: 10.1128/AEM.72.1.638-644.2006.

Yang, H., Gandhi, H., Ostrom, N. E., and Hegg, E. L.: Isotopic fractionation by a fungal P450 nitric oxide reductase during the production of N2O, Environ Sci Technol, 48, 10707-10715, 10.1021/es501912d, 2014.
