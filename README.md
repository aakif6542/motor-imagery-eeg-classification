# Motor Imagery EEG Classification

This project investigates the performance of classical and deep learning methods for EEG-based motor imagery decoding (left vs right hand) using multi-subject data.

## Methods
- **CSP + SVM**: Traditional spatial filtering with linear classification  
- **CNN**: End-to-end deep learning on raw EEG signals  
- **Hybrid Model**: Combination of CSP features with CNN representations  

## Dataset
- BCI Competition IV Dataset 2a  
- Multi-subject EEG recordings  

## Results
| Model       | Accuracy |
|------------|---------|
| CSP + SVM  | ~0.59   |
| CNN        | ~0.88   |
| Hybrid     | ~0.84   |

## Key Findings
- CNN significantly outperformed CSP-based methods  
- CSP showed poor generalization in multi-subject settings  
- Hybrid approach improved over CSP but did not surpass CNN  

## Conclusion
Deep learning models are more effective for motor imagery EEG classification, particularly in handling non-stationary and subject-specific brain signals.

## Motivation
This project explores practical challenges in building robust BCI systems and the transition from traditional signal processing methods to deep learning approaches.
