# ModERFoRest
[![Join the chat at https://gitter.im/cafervero/moderforest](https://badges.gitter.im/cafervero/moderforest.svg)](https://gitter.im/cafervero/moderforest?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

<em>ModERFoRest</em> name is an acronym that stands for <em>Modelling Environmental Requirements for Forest Restoration</em>. This piece of software aims to assist in management decision process or in species distribution studies. Other uses will be tested. It uses environmental niche models to predict species distribution areas, using only presence data and providing statistical validation.

ModERFoRest is composed by three modules <em>(SDM: Species Distribution Modeling; FSR: Forest Stand Resemblance; SSER: Species Suitability for Ecosystem Restoration)</em> and one main core which contains the algorithms used in the different modules. The program also has a small selection of tools. Actually, an environmental variables editor, a species editor and an edhapic variables calculator are available, but it is planned to add a calculator of hydrological datasets and comparisons of environmental niches in comming releases. In the medium term we will use <a href="http://www.gdal.org/">GDAL</a> as well.

ModERFoRest uses Qt C++ libraries in order to be platform agnostic. Nevertheless, only project files for GNU/Linux and MS Windows are available. If you are a Mac OS developer and are interested in forest repopulation, please take a look at [CONTRIBUTING](CONTRIBUTING.md) file and join us!

## ModERFoRest modules
### SDM : Species Distribution Modeling
This module generates maps of probability of occurrence of a particular species from known locations of the species. This module is suitable for large territory extensions such as provinces, states or even whole countries.
Input data:
 - Species presences file (CSV file containing the coordinates of species presence points).
 - Environment variables raster files. These ones could be climatic but climatic and edhapic.
 - Modelling options (algorithm, statistical parameters, validation parameters).

Output data:
 - Raster files with species presence probablities.
 - Raster files with typical deviation, minimum and maximum of these probabilities.
 - Validations of the model: curve of <em>Boyce-Hirzel (Hirzel et al. 2006)</em> and <em>Kolmogorov-Smirnoff</em> test.

### FSR : Forest Stand Resemblance
This module uses similar data inputs of SDM module, but now the points are where we want to calculate the suitability for each of the 19 species of which we have ecological niches.


### SSER : Species Suitability for Ecosystem Restoration
We are working on it. Check it back soon.


## ModERFoRest tools
### Species and environmental variables editors
We are working on it. Check it back soon.

### Edaphic variables calculator
This tool allows calculation of soil variables for each profile from data obtained by horizons. It also allows the calculation of these variables in surface, varying the depth considered superficial.



