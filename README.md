# Motor Imagery EEG Classification

This project explores how different machine learning and deep learning approaches perform on motor imagery EEG data.

The main goal was to understand:
- How traditional methods (CSP + SVM) perform
- Whether deep learning (CNN) can improve performance
- If combining both (hybrid approach) gives better results


## 🧠 What is Motor Imagery?

Motor imagery means imagining movements (like left or right hand) without actually moving.  
These thoughts generate EEG signals, which can be classified using machine learning.


## ⚙️ Methods Used

### 1. CSP + SVM (Baseline)
- Common Spatial Pattern (CSP) for feature extraction  
- Support Vector Machine (SVM) for classification  

### 2. CNN (Deep Learning)
- Convolutional Neural Network trained directly on EEG signals  
- Learns spatial + temporal patterns automatically  

### 3. Hybrid Model
- Combines CSP features with CNN-learned features  
- Final classification using SVM  


## 📊 Dataset

- BCI Competition IV Dataset 2a  
- Multi-subject EEG data  
- Left vs Right hand motor imagery  


## 🧪 Experimental Setup

- Multi-subject training  
- Subject-wise data splitting  
- Proper normalization (train-only statistics)  
- Evaluation using accuracy and confusion matrix  


## 📈 Results

| Model | Accuracy |
|------|--------|
| CSP + SVM | ~0.59 |
| CNN | ~0.88 |
| Hybrid | ~0.84 |


## 🔍 Key Observations

- CNN significantly outperformed traditional CSP-based methods  
- CSP struggled in multi-subject settings (poor generalization)  
- Hybrid model improved over CSP but did not surpass CNN  


## 🧠 Conclusion

Deep learning models are more effective for motor imagery EEG classification, especially in multi-subject scenarios.  
Combining traditional and deep features does not always guarantee improvement.


## 💡 Why this project?

This project was done to explore the transition from traditional ML to deep learning in BCI systems and understand practical challenges in EEG signal classification.

