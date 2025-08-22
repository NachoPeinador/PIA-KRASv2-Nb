# 🧬 PIA-KRASv2-Nb: A High-Affinity Nanobody against KRAS

[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.16578454-blue)](https://doi.org/10.5281/zenodo.16578454)
<a href="https://explore.openaire.eu/search/publication?pid=10.5281%2Fzenodo.16578455">
  <img src="https://img.shields.io/badge/OpenAIRE-Indexed-green" alt="OpenAIRE Indexed">
</a>
![ipTM](https://img.shields.io/badge/ipTM-0.78-blue)
![pTM](https://img.shields.io/badge/pTM-0.92-blue)
[![Platform](https://img.shields.io/badge/Preprint-Research_Square-blue)](https://www.researchsquare.com/article/rs-7239936/v1)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)

This repository documents the *in silico* design and validation of **PIA-KRASv2-Nb**, a therapeutic nanobody targeting the accessible `DEYDPTIEDS` epitope of the KRAS oncoprotein. This work now integrates results from a **10-nanosecond molecular dynamics (MD) simulation**, confirming not only the persistence but also the refinement of the binding interface over physiologically relevant timescales.

![3D Model of PIA-KRASv2-Nb (Seed 72)](https://raw.githubusercontent.com/NachoPeinador/PIA-KRASv2-Nb/main/AlphaFold_images/KRASKILLER.png)
📌 *Structural model generated with AlphaFold-Multimer v3 (seed 72). ipTM = 0.78 | pTM = 0.92*

---

## 🎯 Key Design Principles & Insights

The nanobody's high affinity is driven by two key principles that were validated computationally:

1.  **Electrostatic Complementarity (The "Molecular Magnet")**
    A key finding is the strong charge complementarity at the interface. The nanobody presents a positively charged paratope that is perfectly oriented to neutralize a highly negative "hotspot" on the KRAS epitope, guiding the initial binding.

    ![Electrostatic Complementarity Map](https://raw.githubusercontent.com/NachoPeinador/PIA-KRASv2-Nb/main/Interactions/af_pose_electrostatics_final.png)
    📌 *2D map showing positive (red) and negative (blue) electrostatic potentials, demonstrating the basis for the targeted attraction.*

2.  **Dynamic Stability (The "Molecular Velcro")**
    Once anchored, the binding is secured by a dense and persistent network of interactions, confirmed by a **10 ns MD trajectory**:
    * **RMSD Plateau:** The complex stabilizes at ~2.3 Å and remains tightly bound.
    * **Persistent Contacts:** Over 90% of key interfacial contacts, including the central polar cluster (SER54–GLU24), remain stable across the entire simulation.
    * **Rigid Anchor:** The CDR3 loop shows minimal fluctuations (<0.3 Å), acting as a rigid binding anchor.

    ![Dynamic Stability RMSD Plot](https://raw.githubusercontent.com/NachoPeinador/PIA-KRASv2-Nb/main/MD_Simulation/rmsd_plot.png)
    📌 *10 ns OpenMM simulation — RMSD evolution confirms strong and persistent binding.*

---

## 🚀 Run the Analysis Pipelines in Google Colab

This project provides complete, three-step pipelines. **Run them in order:**

| Step | Description | Link |
| :--- | :---------- | :--- |
| **1** | **MD Simulation** (Run first) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1W2FtbyPI9uDkZCDqqdFkd6nVQfMoj_Kj) |
| **2** | **Trajectory Analysis** (After Step 1) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Aue7oYHIFAmSe5xPwzyUB-HXJ6NgqNVb) |
| **3** | **Electrostatic Analysis** (Static Pose)| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VghJ-0wAsh_N895uYCMhDKcMBpYGW0uY) |

---

## 📂 Repository Contents

* 🇬🇧 [**`PIA-KRASv2-Nb_Report_ENG.pdf`**](./PIA-KRASv2-Nb_Report_ENG.pdf): Full scientific report in English.
* 🇪🇸 [**`PIA-KRASv2-Nb_Report_ESP.pdf`**](./PIA-KRASv2-Nb_Report_ESP.pdf): Full scientific report in Spanish.
* 💻 [**`MD_Pipeline/`**](./MD_Pipeline/): Google Colab notebooks for the MD simulation and analysis.
* 🔬 [**`Interactions_Analysis/`**](./Interactions_Analysis/): Google Colab notebook and resources for static interaction analysis (contacts, SASA, electrostatics).
* 📁 [**`AlphaFold_models/`**](./AlphaFold_models/): 3D structures of the elite seeds (`.cif` format).
* ⚖️ [**`LICENSE.md`**](./LICENSE.md): Detailed project license (CC BY-NC 4.0).

---

## 📈 Key Results Summary

| Parameter | Value | Tool / Method |
| :--- | :--- | :--- |
| **Binding Confidence (ipTM)** | **0.78** | AlphaFold-Multimer v3 (Seed 72) |
| **Dynamic Stability (10 ns MD)** | ✅ **Stable (~2.3 Å plateau)** | OpenMM Simulation |
| **Persistent H-Bonds (10 ns)** | **>5 maintained** | 10 ns trajectory |
| **Humanization (Family)** | ✅ **VH3 Family** | Hu-mAb |
| **CDR3 Stability (RMSD)** | **0.19 Å** | NanoBodyBuilder2 |

---

## 🧪 Proposed Applications

* **Targeted Therapy:** Pan-mutant inhibition of KRAS signaling.
* **Molecular Diagnostics:** Epitope-specific biosensors with high robustness.
* **Protein Engineering:** Scaffold for bivalent/ADC formats with proven stability.

---

## 🤝 Contact & Collaboration

This project is open for experimental validation. If you work in immunotherapy, structural biology, or cellular assays and are interested in collaborating:

### [📧 Nacho Peinador](mailto:joseignacio.peinador@gmail.com)
**ORCID:** [https://orcid.org/0009-0008-1822-3452](https://orcid.org/0009-0008-1822-3452)

---

## 📄 License

Licensed under Creative Commons Attribution-NonCommercial 4.0 International. This work is registered with the Spanish Intellectual Property Registry (RPI) as verifiable proof of authorship. See [LICENSE.md](./LICENSE.md) for terms and conditions for commercial licensing.
