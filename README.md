# Biomedical Data Scientist

#### Technical Skills: Python, MATLAB, R, SQL, AWS, Git, SPM, AFNI

---

## <ins>Education</ins>
B.A., Computational Cog. Sci. | Rice University (_May 2024_)

---

## <ins>Research</ins>
**National Cancer Institute (NCI/NIH) | (_June 2024 - Oct. 2024_)**<br />
*Radiation Oncology Branch*<br />
**Advisors: Andra V. Krauze, Erdal Tasci**

**Baylor College of Medicine | (_Jan. 2024 - May 2024_)**<br />
*Russel S. Ray Lab of Molecular Neurobiology*<br />
**Advisors: Russel S. Ray, Christopher Ward**

**Rice University School of Engineering | (_Aug. 2022 - May 2024_)**<br />
*Rice Data to Knowledge (D2K)*<br />
**Advisors: Bartlett D. Moore, Genevera Allen**

---

## <ins>Projects</ins>

### Navigating Omic Changes by Radiation Therapy in High-Grade Glioma/Glioblastoma

Performed feature extraction, selection and engineering on multi-omic (proteomic, metabolomic) data from patients with pathology proven glioblastoma, a grade 4 brain tumor/glioma. This is in conjunction with research and development of AI models that can assist in revealing potential serum biomarkers, in addition to prediction of tumor characteristics (size, location, morphology, etc.) and patient outcomes. 

<img src="images/Figure 1 NCI.jpg?raw=true" />

The metabolomic data is first put into an RFE w/ K-Fold CV to find the most important features, which are then put into a deep-learning stacked autoencoder to compress the data. The compressed feature space is then put into another Random Forest to evaluate performance.

<img src="images/Figure 2 NCI.jpg?raw=true" />

Once the best parameters and architectures are found, the autoencoder uses only the encoder portion in attempt to reconstruct only one target feature. The target feature can be a compound, giving us insights of which other compounds are most similar to the target.

<img src="images/Figure 3 NCI.jpg?raw=true" />

---
