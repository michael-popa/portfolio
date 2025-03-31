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

### Navigating Omic Changes by Radiation Therapy in High-Grade Glioma/Glioblastoma - _National Cancer Institute_

Performed feature extraction, selection and engineering on multi-omic (proteomic, metabolomic) data from patients with pathology proven glioblastoma, a grade 4 brain tumor/glioma. This is in conjunction with research and development of AI models that can assist in revealing potential serum biomarkers, in addition to prediction of tumor characteristics (size, location, morphology, etc.) and patient outcomes. 

<img src="images/Figure 1 NCI.jpg?raw=true" />

The metabolomic data is first put into an RFE w/ K-Fold CV to find the most important features, which are then put into a deep-learning stacked autoencoder to compress the data. The compressed feature space is then put into another Random Forest to evaluate performance.

<img src="images/Figure 2 NCI.jpg?raw=true" />

Once the best parameters and architectures are found, the encoder is used to reconstruct only one target feature. The target feature can be a compound, giving us insights of which other compounds are most similar to the target.

<img src="images/Figure 3 NCI.jpg?raw=true" />

The result found 30+ novel metabolites that may show promise as biomarkers for glioma.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?logo=scikit-learn&logoColor=white) 
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?logo=scipy&logoColor=%white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?logo=TensorFlow&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?logo=visual-studio-code&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?logo=jupyter&logoColor=white)

<br><br>
<br><br>

---

### Identifying Cardio-Respiratory Signatures of SIDS in Mouse Models - _Baylor College of Medicine_

The underlying mechanisms of SIDS remain elusive due to its unpredictability on pre-mortem data. By leveraging a unique dataset derived from mouse pups simulating SIDS conditions, advanced signal processing techniques were combined with machine learning to analyze cardio-respiratory waveforms, given the hope of potential biomarker discovery.
<br><br>
Raw ECG data was extensively preprocessed to extract meaningful information (e.g., QRS complex morphology) to understand their relationship to SIDS.

<img src="images/QRS Detection Large.jpg?raw=true" />

* **Data**: Readings collected from ~400 mice pups categorized into: Heart data, Breath data and Raw signal data.
* **Feature Selection**: 192 Features collected for each mouse sample → 51 features selected and engineered to predict SIDS.
* **Feature Engineering**: Using the raw ECG signal, the common segments present in a heartbeat interval (the QRS points) were detected.

Two modeling approaches were explored: <br>

(1) A **1D convolutional neural network (CNN) with Long Short-Term Memory (LSTM)** utilizing engineered tabular features.

<img src="images/1D CNN with LSTM.jpg?raw=true" />

(2) A **2D CNN** utilizing spectrograms.

<img src="images/2D CNN.jpg?raw=true" />

The approaches showed great promise for future implementations. Though, the novel nature of this work the data collection was insufficient to accurately conclude model efficacy.
<br><br>
The pipeline automation proved to be successful. Thus, in the coming years, the lab will collect more data and may perform further model analysis.

<br><br>
<br><br>

---

### Predicting Synaptic Activity Based On Axonal-Dendritic Proximity (ADP) - _Rice University_

When the axon of one neuron comes close to the dendrite of another neuron, that is the axonal-dendritic proximity - every synapse results from an ADP, but not every ADP results in a synapse. Thus, we develop a binary classification problem using machine learning to predict ADP-to-synapse conversion.

The activity of neurons in the visual cortex of a mouse were imaged with 2-photon (2P) microscopy, and every neuron was reconstructed in 3D.

<img src="images/ADP.jpg?raw=true" />

The development process involved preprocessing, feature engineering, modeling, hyperparameter tuning, and cross-validation.

<img src="images/Engineered Features.jpg?raw=true" />

The focus was on four predictive modeling techniques: Support Vector Machines (SVMs), Random Forest (RF), Deep-Learning, and Model Stacking.

Model stacking proved to be most predictive with the following algorithms: linear Support Vector Machines, Adaptive Boosting, Gradient Boosting, K-Nearest Neighbors, and Random Forest as base learners, and a linear SVM as a meta learner.

<img src="images/ROC Curve.jpg?raw=true" />

The receiver operating characteristic curve demonstrates great performance for true positives against false positives. 

The effort achieved ∼79.611% accuracy, which was a significant advancement from the expected/traditional score of ∼77% +/-1%. Furthermore, we find the most important feature in synaptic prediction is the depth of the dendritic ADP, alongside the pre-synaptic neuron’s receptive field vertical location.

<br><br>
<br><br>

---
