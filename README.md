# About inventory:
This inventory of atmospheric emissions was developed for four industrial sectors in Brazil (crude oil refining, cement production, pulp and paper, and electricity generation) using a bottom-up approach for the period 1990 to 2022. The analysis includes a comparison with data from the global EDGAR inventory, an assessment of emission factors, spatialization, and the development of R code for automation, updating, and use in air quality models. Estimates are made based on EPA and EEA guidelines, and the results show that the southeast region concentrates the highest emission rates, with emphasis on the electricity generation sector, whose particulate matter emissions exceed those of the EDGAR road transportation sector. The COVID-19 pandemic impacted the cement, pulp and paper, and electricity generation sectors, while the refining sector was less affected. This project provides a robust tool for air quality management in Brazil.

# Available Files:
The “Brazil-industrial-emissions-inventory” repository has the "emissions_data" folder where emissions from the inventoried sectors for Brazil are made available. The files EPA_CEM.txt, EEA_CEM.txt, EPA_PAP.txt, EEA_PAP.txt, EPA_REF.txt, EEA_REF.txt, EPA_TPP.txt and EEA_TPP.txt contain the name of the emitter, the geographic coordinates and the identification of each emitting source. In addition, it includes the emission for original (typical) lower and upper emission factors for TSP, PM10, PM2.5, BC, NOx, CO, NMVOCs, and SOx, in Gg/year for the base years from 1990 to 2023. The "factors" folder contains the activity factors used to estimate emissions

# Updated version - emissions' height
For the representation of chimney heights in the gas and particulate emission records of the country’s four main industrial sectors (cement, thermoelectric power plants, pulp and paper, and oil refineries), a two-step strategy was adopted to address the limited availability of detailed data in existing inventories.
In the first stage, automation in R added a column with a representative average chimney height for each sector. For the cement industry, due to the absence of national data, a value of 115 m was used as a proxy for large-scale facilities, based on international references (Table 1). The resulting base files were saved with the suffix _ALT.txt.
The second stage involved manual refinement, where the average values were replaced with specific height data collected from identified facilities in previous studies (Table 1). This step ensured greater accuracy, and the updated files, combining both representative and specific values, were stored with the suffix _ALT2.txt.

Table 1. Representative chimney heights adopted for each industrial sector
| Name of Industry/Project     | Sector         | Chimney Height (m)    | Data Source                                                                     |
| ---------------------------- | -------------- | --------------------- | ------------------------------------------------------------------------------- |
| UTE Pampa Sul (Candiota, RS) | Thermoelectric | 195                   | OE MAGAZINE. *Cobrazil: Complex logistics to assemble a 200 m chimney.*         |
| Pecém Power Plant (CE)       | Thermoelectric | 150 (one) / 110 (two) | STRUCTURAL ENGINEERING. *Chimneys for thermoelectric plants.* Londrina, 2009.   |
| Itaqui Power Plant (MA)      | Thermoelectric | 110                   | STRUCTURAL ENGINEERING. *Chimneys for thermoelectric plants.* Londrina, 2009.   |
| Bracell (Star Project)       | Pulp and Paper | 147.3                 | TEMEC Forms and Scaffolding. *Case — Bracell Exhaust Chimney.*                  |
| Cement Industries (general)  | Cement         | 115                   | WARWICKSHIRE COUNTY COUNCIL. *Climafuel Facility at Malpass Farm, Rugby.* 2013. |
| Oil Refineries (general)     | Oil Refining   | 40–110                | Steelcon / Dominion Steelcon A/S. *Chimneys for a refinery.*                    |


# Citation and more information:
Ibagué-Rey et al. (2025). A comprehensive atmospheric emissions inventory for major Brazilian industrial sectors: a bottom-up approach with spatial distribution analysis.
link: https://doi.org/10.1080/09593330.2025.2560588

Ibagué Rey et al. (2023). Development of an atmospheric emissions inventory for four industrial sectors of Brazil with a bottom-up approach.
link: https://riut.utfpr.edu.br/jspui/bitstream/1/32339/1/inventarioemissoesindustriaisbrasil.pdf


# Communications, doubts etc:
e-mail: martinsld@yahoo.com
