 # 🧪 OpenADMET 
 ### — AI-Powered ADMET & Drug Safety Prediction
AI-driven ADMET, pharmacokinetics, and toxicity prediction for early drug discovery
#### Our Team: Xichen(Mint) Zhang, Yizhou Ma, Xin Chen 

##


## 🔗 Quick Links
#### 🌐 Website: https://yourcompany.com/openadmet
#### 💼 LinkedIn: https://www.quanta-bricks.com/
#### 📄 Paper: https://chemrxiv.org/doi/10.26434/chemrxiv.15001004 
#### 📝 Blog: https://www.linkedin.com/feed/update/urn:li:activity:7464319820725948416/




## Introduction to OpenADMET
OpenADMET is a collaborative, open-science initiative designed to improve drug discovery by tackling the unpredictable pharmacokinetic and toxicity profiles of small molecules. Backed by organizations like the Open Molecular Software Foundation, it provides public datasets, machine learning models, and regular blind challenges to standardize and advance ADMET modeling.

🧬 What is OpenADMET?
OpenADMET provides fast, accurate, and interpretable AI models to predict key drug safety and pharmacokinetic properties, helping accelerate early-stage drug discovery.
Key Predictions
#### ✅ Absorption: Oral bioavailability, permeability (Caco-2), P-gp substrate
#### ✅ Distribution: Plasma protein binding, VD
#### ✅ Metabolism: CYP450 inhibition/induction, metabolic stability
#### ✅ Excretion: Renal clearance
#### ✅ Toxicity: Hepatotoxicity, cardiotoxicity (hERG), genotoxicity, carcinogenicity

## ⚠️ Key Challenges We Solved
ADMET prediction remains a major bottleneck in early drug discovery due to several long-standing challenges:
#### 1. Low-quality and scarce labeled data. 
Public ADMET datasets are small, noisy, and inconsistently annotated, leading to poor generalization of traditional models.
#### 2. Inadequate molecular representation: 
Single fingerprints or descriptors fail to capture 3D structure, electronic effects, and chiral information critical for accurate prediction.

#### 3.Multi-task conflicts and uneven performance. 
ADMET involves over 10 sub-tasks. Conventional models struggle with multi-task trade-offs, resulting in inconsistent accuracy across endpoints.

#### 4. Black-box models with limited interpretability.
Pure deep learning approaches lack transparent reasoning, making results hard to trust and adopt in industrial decision-making.

#### 5.High deployment barriers for real-world use.
Existing tools are either closed-source and expensive or open-source but low in accuracy, rarely balancing performance and practicality.

##

#### How OpenADMET addresses these challenges: 
A unified framework integrating multi-modal molecular representation, multi-task collaborative training, attention-based interpretability, and lightweight deployment, delivering robust, reliable, and production-ready ADMET predictions.

 
### QuantaBricks 
https://www.quanta-bricks.com/

Recently, our team placed 85th among 370+ global participants in the OpenADMET prediction challenge. The project was designed as a stress test for extreme model compression — operating under strict parameter limits, single-core CPU execution, and without quantum chemical descriptors.

Coming from an applied mathematics background, stepping into AI-driven drug discovery pushed me to think deeply about representation design under real-world computational constraints. Learning organic chemistry fundamentals and SMILES representations while experimenting with fingerprint compression, VAE, late fusion, and Mixture of Experts broadened my perspective on how modeling choices shape performance in biomedical AI. 


## Negative Findings
### Faliure Models
### Limitations
#### 1. Limited to small molecules

OpenADMET does not support peptides, antibodies, oligonucleotides, or large biologics.

#### 2.Does not model dynamic biological processes

The model predicts static properties but cannot simulate time-dependent pharmacokinetics or in vivo dynamics.

#### 3. Dependent on data quality
 Performance may degrade for novel, rare, or under-represented scaffolds not well-covered in training data.
   
#### 4. Lack of organ-level or tissue-specific simulation
Current version provides holistic predictions without tissue-specific resolution (e.g., liver vs. kidney metabolism).
   
#### 5. Does not include drug–drug interaction (DDI) or metabolism cascade prediction
These complex biological behaviors require external models or future extensions.
   
#### 6. In silico predictions are not fully equivalent to clinical results
 All outputs must be validated by in vitro and in vivo experiments before practical use.

### Assumption

#### 1. SMILES-based molecular representation is sufficient 
for predicting ADMET properties. 3D conformation is not required for most in silico ADMET tasks.

#### 2. Public and curated datasets are biologically representative 
of real-world compound behavior in wet-lab experiments.

#### 3. ADMET endpoints are partially correlated 
and can be learned together via multi-task learning.

#### 4. Molecular structure alone determines ADMET profile 
without considering disease state, patient population, or drug–drug interactions in the current version.

#### 5. Label noise in public datasets can be alleviated 
by robust training strategies and ensemble learning.

### Generalization / Generalizability (泛化能力)
#### 1. Cross-scaffold generalization: 
The model generalizes to unseen molecular scaffolds by learning global physicochemical and topological rules.

#### 2. Multi-dataset robustness
OpenADMET is trained on diverse, high-quality ADMET databases and maintains stable performance across external test sets.

#### 3. Low-data adaptation
The multi-task architecture enables reasonable performance even for tasks with limited labeled data.

#### 4. Applicable to real-world drug-like molecules
The model is validated on drug-like compounds rather than only idealized molecules, supporting real discovery scenarios.


###  Biological Mechanism（生物机理）
Biological Mechanism
OpenADMET captures biologically meaningful patterns during training, enabling interpretable ADMET predictions:

#### 1.Molecular structure → physicochemical properties → ADMET behavior
The model learns lipophilicity, polarity, molecular size, flexibility, and electronic properties that drive absorption, distribution, and metabolism.

#### 2.Binding affinity & enzyme interaction
For CYP450, hERG, and protein binding tasks, the model infers binding potential via structural motifs.









