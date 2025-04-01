# Michael Popa

#### Technical Skills: Python, MATLAB, R, SQL, AWS, Git, SPM, AFNI

---

## Education
B.A., Computational Cog. Sci. | Rice University (_May 2024_)

---

## Research
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

## Projects

### Navigating Omic Changes by Radiation Therapy in High-Grade Glioma/Glioblastoma - _National Cancer Institute_

Performed feature extraction, selection and engineering on multi-omic (proteomic, metabolomic) data from patients with pathology proven glioblastoma, a grade 4 brain tumor/glioma. This is in conjunction with research and development of AI models that can assist in revealing potential serum biomarkers, in addition to prediction of tumor characteristics (size, location, morphology, etc.) and patient outcomes.

The high-dimensional dataset consisted of 6,015 metabolomic features with only 214 patient serum samples.

<img src="images/Figure 1 NCI.jpg?raw=true" class="nci" />

The metabolomic data is first put into an RFE w/ K-Fold CV to find the most important features, which are then put into a deep-learning stacked autoencoder to compress the data. The compressed feature space is then put into another Random Forest to evaluate performance.

<img src="images/Figure 2 NCI.jpg?raw=true" class="nci" />

Once the best parameters and architectures are found, the encoder is used to reconstruct only one target feature. The target feature can be a compound, giving us insights of which other compounds are most similar to the target.

<img src="images/Figure 3 NCI.jpg?raw=true" class="nci" />

The result found 30+ novel metabolites that may show promise as biomarkers for glioma.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)
[![NumPy](https://img.shields.io/badge/NumPy-4DABCF?logo=numpy&logoColor=fff)](#)
[![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=fff)](#)
[![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?logo=matplotlib&logoColor=fff)](#)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?logo=scikit-learn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?logo=scipy&logoColor=%white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?logo=TensorFlow&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?logo=visual-studio-code&logoColor=white)

<br><br>
<br><br>

---

### Identifying Cardio-Respiratory Signatures of SIDS in Mouse Models - _Baylor College of Medicine_

The underlying mechanisms of SIDS remain elusive due to its unpredictability on pre-mortem data. By leveraging a unique dataset derived from mouse pups simulating SIDS conditions, advanced signal processing techniques were combined with machine learning to analyze cardio-respiratory waveforms, given the hope of potential biomarker discovery.
<br><br>
Raw ECG data was extensively preprocessed to extract meaningful information (e.g., QRS complex morphology) to understand their relationship to SIDS.

<img src="images/QRS Detection Large.jpg?raw=true" class="bcm" />

* **Data**: Readings collected from ~400 mice pups categorized into: Heart data, Breath data and Raw signal data.
* **Feature Selection**: 192 Features collected for each mouse sample → 51 features selected and engineered to predict SIDS.
* **Feature Engineering**: Using the raw ECG signal, the common segments present in a heartbeat interval (the QRS points) were detected.

Two modeling approaches were explored: <br>

(1) A **1D convolutional neural network (CNN) with Long Short-Term Memory (LSTM)** utilizing engineered tabular features.

<img src="images/1D CNN with LSTM.jpg?raw=true" class="bcm" />

(2) A **2D CNN** utilizing spectrograms.

<img src="images/2D CNN.jpg?raw=true" class="bcm" />

The approaches showed great promise for future implementations. Though, the novel nature of this work the data collection was insufficient to accurately conclude model efficacy.
<br><br>
The pipeline automation proved to be successful. Thus, in the coming years, the lab will collect more data and may perform further model analysis.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)
[![NumPy](https://img.shields.io/badge/NumPy-4DABCF?logo=numpy&logoColor=fff)](#)
[![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=fff)](#)
[![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?logo=matplotlib&logoColor=fff)](#)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?logo=scikit-learn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?logo=scipy&logoColor=%white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?logo=TensorFlow&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?logo=visual-studio-code&logoColor=white)
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)](#)
[![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=fff)](#)

<br><br>
<br><br>

---

### Predicting Synaptic Activity Based On Axonal-Dendritic Proximity (ADP) - _Rice University_

When the axon of one neuron comes close to the dendrite of another neuron, that is the axonal-dendritic proximity - every synapse results from an ADP, but not every ADP results in a synapse. Thus, we develop a binary classification problem using machine learning to predict ADP-to-synapse conversion.

The activity of neurons in the visual cortex of a mouse were imaged with 2-photon (2P) microscopy, and every neuron was reconstructed in 3D.

<img src="images/ADP.jpg?raw=true" />

The data transformation steps include: resampling (SMOTE, Undersampling, bootstrapping), feature selection (RFE, Lasso, Tree-based), dimensionality reduction, and feature engineering.

<img src="images/Engineered Features.jpg?raw=true" />

The focus was on four predictive modeling techniques: Support Vector Machines (SVMs), Random Forest (RF), Deep-Learning, and Model Stacking.

Model stacking proved to be most predictive with the following algorithms: linear Support Vector Machines, Adaptive Boosting, Gradient Boosting, K-Nearest Neighbors, and Random Forest as base learners, and a linear SVM as a meta learner. Validated through Randomized and GridSearch cross-validation.

<p align="center">
  <img src="images/ROC Curve.jpg?raw=true" style="width: 75%; height: 75%;" />
</p>

The receiver operating characteristic curve demonstrates great performance for true positives against false positives. 

The effort achieved ∼79.611% accuracy, which was a significant advancement from the expected/traditional score of ∼77% +/-1%. Furthermore, the runtime was considered the lowest of all traditional implementations (~2.6 min.). Lastly, we find the most important feature in synaptic prediction is the depth of the dendritic ADP, alongside the pre-synaptic neuron’s receptive field vertical location.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)
[![NumPy](https://img.shields.io/badge/NumPy-4DABCF?logo=numpy&logoColor=fff)](#)
[![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=fff)](#)
[![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?logo=matplotlib&logoColor=fff)](#)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?logo=scikit-learn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?logo=PyTorch&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?logo=TensorFlow&logoColor=white)
![Jupyter Notebook](https://camo.githubusercontent.com/55b0c06404092071078dabdf9cc39b52a40ba653415dde70919cae77628f8cca/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4a7570797465722d4c61622d4633373632362e7376673f7374796c653d666c6174266c6f676f3d4a757079746572)

<br><br>
<br><br>

---

### Memory Performance and Hippocampal Volume: A Simulation of Visual Encoding and Retrieval - _Rice University_

The relationship between memory performance and hippocampal volume remains a debate. Thus, by simulating appropriate limbic system structures (entorhinal + temporal cortex, DG, CA3, CA1) in a 2D Covolutional Autoencoder model, we may find unique changes in visual encoding and retrieval based on layer variation.

<img src="images/Hippocampus.jpg?raw=true" />

The data consisted of  70,000 28x28 black and white images from 10 clothing categories. By targeting lesions in various subregions of the medial temporal lobe, we have a clearer idea of how that impacts memory performance of visual stimuli.

This is an example of how visual details can be lost during retrieval over time:

<img src="images/Retrieval Example.jpg?raw=true" />

The findings suggest hippocampal volume **does** play a role in memory performance, depending heavily on the specific layer that is damaged. Further, the model shows that the ability to generalize a visual stimulus does not come solely from the shape and structure but also from the shade of the image.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff)
[![NumPy](https://img.shields.io/badge/NumPy-4DABCF?logo=numpy&logoColor=fff)](#)
[![Matplotlib](https://custom-icon-badges.demolab.com/badge/Matplotlib-71D291?logo=matplotlib&logoColor=fff)](#)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?logo=Keras&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?logo=TensorFlow&logoColor=white)
[![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab&logoColor=fff)](#)
![Jupyter Notebook](https://camo.githubusercontent.com/55b0c06404092071078dabdf9cc39b52a40ba653415dde70919cae77628f8cca/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4a7570797465722d4c61622d4633373632362e7376673f7374796c653d666c6174266c6f676f3d4a757079746572)

<br><br>
<br><br>

---

### Multivariate Data Analysis of Linguistic Biomarkers for Parkinson’s Disease (PD) - _Rice University_

As Parkinson's disease is known to target older individuals, it is key to identify the onset of the disease as quick as possible. Hlavnička et al. (2017) sought to uncover early biomarkers of PD in patients with rapid eye movement sleep behavior disorder (RBD), as they are at high risk of developing PD.

Therefore, their speech patterns, if similar to PD patients, could be considered early biomarkers of Parkinson's. The participants perform a series of tasks, and a number of linguistic characteristics are measured.

In R, we perform ANOVA testing with a Tukey Honest Significance Difference on three groups: PD, RBD, and a control group. The following animated box plots can show the results:

<p align="center">
  <img src="images/Rate of Speech Timing CROPPED.gif?raw=true" style="width: 80%; height: 80%;" />
</p>
---

<p align="center">
  <img src="images/Duration of Unvoiced Stops CROPPED.gif?raw=true" style="width: 80%; height: 80%;" />
</p>

---

<p align="center">
  <img src="images/Duration of Pause Intervals CROPPED.gif?raw=true" style="width: 80%; height: 80%;" />
</p>

Further, a variety of statistical tests and analysis is performed, such as Pearson correlation, R-squared, linear regression, t-test, and an f-statistic.

Taking into account age, we can create an interactive box plot. Here's an example specifically for the reading task of the participants:

<iframe src="https://michael-popa.github.io/Reading%20a%20Passage%20Age%20Group.html" width="100%" height="500px"></iframe>




