# SWMM-Based Spore Transport Model for Emergency Response Planning

This repository contains scripts and supporting documentation related to the study:

> **Using SWMM for emergency response planning: A case study evaluating biological agent transport under various rainfall scenarios and urban surfaces**  
> *Yuan, L., Mikelonis, A.M., Yan, E. (2023). Journal of Hazardous Materials, 458, 131747.*  
> [DOI: 10.1016/j.jhazmat.2023.131747](https://doi.org/10.1016/j.jhazmat.2023.131747)

## 📌 Project Overview

This work demonstrates the use of the **Storm Water Management Model (SWMM)**—specifically **PCSWMM with IronPython scripting**—for simulating the fate and transport of *Bacillus anthracis* surrogate spores following hypothetical contaminant releases in an urban environment. The modeling approach supports emergency preparedness for biological agent incidents, enabling planners to:

- Visualize contaminant migration pathways
- Identify potential hotspot areas
- Evaluate how land use and rainfall intensity affect spore washoff

## 🛠 Key Components

- **Modeling Tool**: PCSWMM v7.5 using EPA SWMM 5.1.015 engine
- **Code**: Custom IronPython 2.7 script for exporting time-series spore data from selected conduits (`export_flow.py`)
- **Calibration**: Washoff coefficients were derived from observed spore concentrations on asphalt, grass, and concrete surfaces
- **Simulations**:
  - Field experiment release (3 rainfall events)
  - Hypothetical plume scenario (3 rainfall events)

## 🔬 Study Highlights

- Developed a high-resolution stormwater model with 80,000+ subcatchments and 220,000+ conduits
- Calibrated exponential washoff functions using real field data
- Demonstrated that concrete surfaces produced significantly higher spore washoff than asphalt or grass
- Identified critical pathways and outfalls affected under extreme precipitation

@article{Yuan2023SWMM,
  title = {Using SWMM for emergency response planning: A case study evaluating biological agent transport under various rainfall scenarios and urban surfaces},
  author = {Yuan, Lifeng and Mikelonis, Anne M. and Yan, Eugene},
  journal = {Journal of Hazardous Materials},
  volume = {458},
  year = {2023},
  pages = {131747},
  doi = {10.1016/j.jhazmat.2023.131747}
}
