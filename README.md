# Caatinga_Invasive_Plants_ML

Machine-learning classification of non-native plant species in the Brazilian Caatinga dry forest. This repository includes the raw data, predictors, functional traits, phylogenetic metrics, and Google Colab notebooks used to model naturalization and invasion stages using ML and SHAP analyses.

## Data
1. `nonnative_plant_caatinga_ML.txt` – Raw species data

### Predictors
| Variable       | Explanation                                                                                       |
|----------------|---------------------------------------------------------------------------------------------------|
| LA             | Leaf area of the species                                                                          |
| SM             | Seed mass of the species                                                                          |
| H              | Mean height of the species                                                                        |
| PDmin          | Phylogenetic distance to the nearest native which co-occurs with the non-native species           |
| MPD            | Mean phylogenetic distance from the non-native species to all co-occurring native species         |
| MPDw           | Mean phylogenetic distance from the non-native species to all co-occurring native species, weighted by the relative frequency of native plants |
| MRT            | Time in years between the year of introduction and 2024                                          |
| Bio (1:19) native | Average value of each bioclimatic variable in the native range                                   |
| Bio (1:19) diff   | Difference between the average value of each bioclimatic variable in the native range and the average of occurrences in Caatinga |
| NMI            | Average of the environmental distance of each occurrence in Caatinga to the nearest margin of the native niche |
| Euclid         | Mean Euclidean distance between native and non-native range with bioclimatic variables           |
| Pseudo-F       | Pseudo-F of a PERMANOVA between native and non-native range with bioclimatic variables           |
| Area           | Area in squared kilometers in Caatinga predicted by ENM                                          |

## Notebooks
1. `Invasion_Caatinga_ML.ipynb` – Machine learning model for the invasion process
2. `Naturalization_Caatinga_ML.ipynb` – Machine learning model for the naturalization process

## How to Use
- Open the notebooks in Google Colab
- Install required packages
- Follow each notebook step to reproduce the analyses
