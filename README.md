# Socio-hydrological resilience dataset Mexico city and Metropolitan Area

Original Publish Date: 26 May, 2021  
Updated on: 26 May, 2021

This page describes the technical specifications of the *Socio-hydrological resilience dataset for Mexico city and its Metropolitan Area*. The data is presented as geometric polygon features representing the administrative areas.

## Methodology

This research project was developed by the British Geological Survey, the Architectural Association, the Centre for Advanced Spatial Analysis and Fluxus. For more information about the project and methodology visit the project [website](https://www.mexicoshr.com/){target="\_blank"}.

## General description

The dataset comprises a set of variables that describe socio-hydrological vulnerability and the effects of building constructed wetlands for geographic areas called Colonias (n = 2785). Additionally, the effects of constructed wetlands are summarised at larger administrative areas called Alcaldias (n = ). The variables represent a description of the baseline (no constructed wetlands) for the **actual 2020 and future 2050** situations and the estimation of the impacts of **4 budgets schemes**. Socio-hydrological vulnerability is represented by a **Socio-hydrological index (SHI)** which is the quotient between the **Water Stress index (WSI)** and the **Adaptive Capacity index (ACI)**.

The impact of **Constructed Wetlands (CW)** in each Colonia is presented as the total amount of CW measured in square meters, and measured as total budget when this variable is aggregated to Alcaldias. Finally, the indexes and effects of CW (SHI, WSI, ACI and CW) are calculated for **3 world-views scenarios; Stakeholder, Environmental and Social**. As illustrated in the data-cube figure below the combination of these parameters make up 120 variables for Colonias and 30 variables for Alcaldias (budget 0 variables for CW should be removed as this budget produces no impact making a final total of 114 and 24 variables)

<img src="data_cube.png" width="600" style="margin:0px 0px"/>

## Codebook

The name of the variables is created from a string of the different parameters according to the following table. For example, the variable "ACI_c\_w1_b1" corresponds to Adaptive Capacity index for 2020, Stakeholder weighting and budget 1

| Variable name | Variable description                                      |
|---------------|-----------------------------------------------------------|
| ID_Colonia    | unique numeric identifier for Colonia                     |
| Municipality  | Name of Alcaldia (similar to Borough)                     |
| Colonia       | Name of Colonia (similar to LSOA)                         |
| pop           | Total population (by Colonia)                             |
| SHI           | Socio-hydrological vulnerability index                    |
| WSI           | Water Stress index                                        |
| ACI           | Adaptive Capacity index                                   |
| CW_sqm        | Constructed Wetlands in square metres                     |
| c             | current 2020                                              |
| f             | future 2050                                               |
| w1            | Stakeholder (weighting)                                   |
| w2            | Environmental (weighting)                                 |
| w3            | Social (weighting)                                        |
| b0            | no constructed wetlands                                   |
| b1            | 10,000 constructed wetlands                               |
| b2            | 100,000 constructed wetlands                              |
| b3            | 500,000 constructed wetlands                              |
| b4            | maximum constructed wetlands                              |
| cl            | class. The index (SHI, WSI, ACI) reclassified into levels |

## NA values

Occasionally some variables show a NA values. This occurs when it was not possible to compute the value due to missing data or when there is no constructed wetland built.

## Files

The files containing the data are detailed below
