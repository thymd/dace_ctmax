# README

# Data for the article "Upper thermal tolerance differs between populations of a cyprinid fish, *Pseudaspius sachalinensis*."

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19625081.svg)](https://doi.org/10.5281/zenodo.19625081)

---

## Overview

This dataset accompanies the article "Upper thermal tolerance differs 
between populations of a cyprinid fish, *Pseudaspius sachalinensis*." 
The study experimentally evaluated the upper thermal tolerance of 
*P. sachalinensis* using critical thermal maximum (CTmax) measurements 
on fish collected from two tributaries in Hokkaido, Japan, that differ 
in thermal variability but share similar mean water temperatures. 
The dataset comprises water temperature records from the two 
study tributaries, water temperature records from the laboratory 
acclimation tanks, and the individual-level CTmax measurements together 
with morphological data.

## Data files

The dataset consists of three CSV files, each corresponding to a 
different component of the study.

### 1. `d_field_temp.csv` — Water temperature data

Hourly water temperature records from temperature loggers deployed in 
the two study tributaries from 31 July to 14 August 2025. 

| Column       | Description                                                              |
|--------------|--------------------------------------------------------------------------|
| `date_time`  | Date and time of the measurement (`YYYY-MM-DD HH:MM:SS`, JST/UTC+9)      |
| `population` | Source population (`Kerimai` or `Ishikari`)                              |
| `temp`       | Water temperature (°C)                                                   |

### 2. `d_acclimation_temp.csv` — Laboratory acclimation tank temperature data

Hourly water temperature records from the two laboratory tanks in which 
fish from each population were acclimated before the CTmax experiments. 

| Column       | Description                                                              |
|--------------|--------------------------------------------------------------------------|
| `date_time`  | Date and time of the measurement (`YYYY-MM-DD HH:MM:SS`, JST/UTC+9)      |
| `population` | Population assigned to the tank (`Kerimai` or `Ishikari`)                |
| `temp`       | Water temperature in the acclimation tank (°C)                           |

### 3. `d_ctmax.csv` — Individual-level CTmax measurements

Results of the CTmax experiments. 

| Column        | Description                                                                                  |
|---------------|----------------------------------------------------------------------------------------------|
| `population`  | Source population (`Kerimai` or `Ishikari`)                                                  |
| `trial`       | Trial ID                                                                                     |
| `date`        | Date on which the CTmax trial was conducted (`YYYY-MM-DD`)                                   |
| `start_time`  | Time at which the trial started, i.e., when heating began                                    |
| `end_time`    | Time at which the individual reached CTmax and the trial was terminated for that individual  |
| `CTmax`       | Critical thermal maximum: water temperature (°C) at which the individual lost equilibrium    |
| `SL`          | Standard length of the individual (mm), measured to the nearest 1 mm                         |
| `BW`          | Body weight of the individual (g)                                                            |
| `condition`   | Individual body condition                                                                    |

## License

This dataset is released under the Creative Commons Attribution 4.0 
International License (CC BY 4.0). You are free to share and adapt 
the material for any purpose, including commercially, provided that 
appropriate credit is given to the original authors, a link to the 
license is provided, and any changes made are indicated. The full 
license text is available in the `LICENSE.txt` file accompanying this 
dataset, and at https://creativecommons.org/licenses/by/4.0/.

When using this dataset, please cite the original article.
