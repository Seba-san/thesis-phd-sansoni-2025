
# PhD Thesis: Spatio-temporal Reconstruction of Crops using Active Sensing Strategies

**Author:** [Sebastian Sansoni](https://github.com/Seba-san)  
**University:** Universidad Nacional de San Juan (UNSJ), Facultad de Ingeniería  
**Degree:** Doctor en Ingeniería de Sistemas de Control (PhD in Control Systems Engineering)  
**Date:** July 23, 2025

[![YouTube](https://img.shields.io/badge/YouTube-Watch%20Oral%20Defense-red?style=for-the-badge&logo=youtube)](https://www.youtube.com/watch?v=Yeiy6F6qobs)
[![Google Drive](https://img.shields.io/badge/Google%20Drive-Complementary%20Info-blue?style=for-the-badge&logo=googledrive)](https://drive.google.com/drive/folders/1PaDA3Spn4uclJ2oCiJ0T3QvzSgoqvLra?usp=drive_link)

---

## Abstract

Effective uncertainty management is crucial and challenging in Active SLAM (ASLAM), where optimal decision-making for autonomous exploration and mapping is an NP-hard problem. Critical applications such as service robotics or Search and Rescue (SAR) demand reliable maps, yet traditional approaches based on occupancy grids and Classical Frontiers (CF) often lack robust mechanisms to represent, evaluate, and exploit map and agent uncertainty.

This thesis introduces a novel theoretical framework grounded in **Dispersion Probabilities (PD)**, a flexible and interpretable probabilistic metric (PD ∈) proposed to quantify the local uncertainty of robotic estimates relative to user-defined tolerances. From PD, a spatial **Uncertainty Map (UM)** is constructed, which in turn allows for the definition of two original tools: **Uncertainty Frontiers (UF)** and the **SiREn index (Signed Relative Entropy)**. The UF, detected by high gradients in the UM and conditioned by a maximum tolerable uncertainty threshold (σ_max), generalize CF to guide not only the exploration of the unknown but also the re-exploration of mapped areas with high uncertainty, facilitating loop closures. The SiREn index, based on KL-divergence, provides a global metric to quantitatively evaluate map quality, balancing coverage and low uncertainty.

The framework's viability and utility were validated through 2D simulations, which demonstrated the superiority of UF-based planners over CF-based ones in terms of final map quality (evaluated by SiREn), and through the analysis of real 3D data from a complex agricultural environment using an adapted SLAM system that provides 6DOF uncertainty (estimated via PD). This 3D analysis confirmed the ability of UF to identify regions requiring improvement and the utility of SiREn to assess the impact of data quality and uncertainty criteria (σ_max) on the final reconstruction.

---

## Resumen

La gestión eficaz de la incertidumbre es crucial y desafiante en SLAM Activo (ASLAM), donde la toma de decisiones óptimas para la exploración y el mapeo autónomo es un problema NP-hard. Aplicaciones críticas como la robótica de servicios o la Búsqueda y Rescate (SAR) demandan mapas fiables, pero los enfoques tradicionales basados en mapas de ocupación y Fronteras Clásicas (FC) a menudo carecen de mecanismos robustos para representar, evaluar y explotar la incertidumbre del mapa y del agente.

Esta tesis introduce un marco teórico novedoso fundamentado en las **Probabilidades de Dispersión (PD)**, una métrica probabilística (PD ∈) flexible e interpretable propuesta para cuantificar la incertidumbre local de las estimaciones robóticas relativa a tolerancias definidas por el usuario. A partir de las PD, se construye un **Mapa de Incertidumbre (MI)** espacial, que a su vez permite definir dos herramientas originales: las **Fronteras de Incertidumbre (FI)** y el **índice SiREn (Entropía Relativa con Signo)**. Las FI, detectadas por altos gradientes en el MI y condicionadas por un umbral de incertidumbre máxima tolerable (σ_max), generalizan las FC para guiar no solo la exploración de lo desconocido, sino también la re-exploración de áreas mapeadas con alta incertidumbre, facilitando cierres de lazo. El índice SiREn, basado en la divergencia KL, proporciona una métrica global para evaluar cuantitativamente la calidad del mapa, balanceando cobertura y baja incertidumbre.

La viabilidad y utilidad del marco se validaron mediante simulaciones 2D, que demostraron la superioridad de planificadores basados en FI sobre los basados en FC en términos de calidad del mapa final (evaluado por SiREn), y mediante el análisis de datos reales 3D de un entorno agrícola complejo, utilizando un sistema SLAM adaptado que proporciona incertidumbre 6DOF (estimada vía PD). Este análisis 3D confirmó la capacidad de las FI para identificar regiones que requieren mejora y la utilidad de SiREn para evaluar el impacto de la calidad de los datos y los criterios de incertidumbre (σ_max) en la reconstrucción final.

---

## Repository Content

This repository contains all the materials related to the PhD thesis. The main components are:

*   **`/manuscript`**: The complete thesis document in PDF format.
*   **`/code`**: Source code for the simulations, experiments, and analysis developed in this work.
*   **`/presentation`**: Slides used for the oral defense.
*   **`/data`**: Datasets used in the experiments. *(Note: Please check the Google Drive link for larger datasets).*


---

## Code Implementation: `treeSLAM` Repository

This repository contains the manuscript and supporting documents for the PhD thesis. The source code for the 3D SLAM system developed for agricultural environments and used in the experimental validation (Chapter 4) is located in its own dedicated repository:

➡️ **[github.com/Seba-san/treeSLAM](https://github.com/Seba-san/treeSLAM)**

The `treeSLAM` repository includes the implementation of the modules for:
*   Ground plane estimation.
*   Crop row detection.
*   Longitudinal position estimation using artificial landmarks.
*   Final 6DOF pose estimation with uncertainty.

---

## Publications

The following papers were published as part of this doctoral research:

1.  **Sansoni, S., Gimenez, J., Castro, G.I, Tosetti, S., Capraro, F. (2025). Optimizing Exploration with a New Uncertainty Framework for Active SLAM Systems.** *Robotics and Autonomous Systems*.
2.  **Gimenez, J., Sansoni, S., Tosetti, S., Capraro, F., & Carelli, R. (2022). Trunk detection in tree crops using RGB-D images for structure-based ICM-SLAM.** *Computers and Electronics in Agriculture*.

---

## How to Cite

If you use this work, please cite the thesis and/or the relevant publications.

### Citing the Thesis

```
@phdthesis{sansoni2025thesis,
  author  = {Sebastian Sansoni},
  title   = {Reconstrucción espacio-temporal de cultivos utilizando estrategias de sensado activo},
  school  = {Universidad Nacional de San Juan},
  year    = {2025},
  month   = {July}
}
```

### Citing the Publications

```bibtex
@article{sansoni2025optimizing,
  title={Optimizing exploration with a new uncertainty framework for active SLAM systems},
  author={Sansoni, Sebastian and Gimenez, Javier and Castro, Gast{\'o}n and Tosetti, Santiago and Capraro, Flavio},
  journal={Robotics and Autonomous Systems},
  volume={193},
  pages={105059},
  year={2025},
  publisher={Elsevier}
}

@article{gimenez2022trunk,
  title={Trunk detection in tree crops using RGB-D images for structure-based ICM-SLAM},
  author={Gimenez, Javier and Sansoni, Sebastian and Tosetti, Santiago and Capraro, Flavio and Carelli, Ricardo},
  journal={Computers and Electronics in Agriculture},
  volume={199},
  pages={107099},
  year={2022},
  publisher={Elsevier}
}
```
