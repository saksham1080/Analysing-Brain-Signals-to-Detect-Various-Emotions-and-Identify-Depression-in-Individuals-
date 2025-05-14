# Analysing Brain Signals to Detect Various Emotions and Identify Depression in Individuals

![Brain Signals Visualization](images/banner.png)

## Project Overview
This project analyzes electroencephalogram (EEG) signals to classify emotional states and detect potential indicators of depression. Using deep learning techniques, we process spectral features from brain signals to identify patterns corresponding to different emotional states (Negative, Neutral, Positive).

## Key Features
- 3-class emotion classification system
- Comparative analysis of LSTM, GRU, and DNN models
- Spectral feature analysis of EEG signals
- Depression risk assessment through emotional pattern recognition

## Dataset
- Contains spectral features from EEG signals
- 2,548 frequency-domain features per sample
- 3 balanced emotional classes: 
  - Negative 😠 
  - Neutral 😐 
  - Positive 😃
- Sample visualization of spectral features:

![EEG Feature Visualization](images/feature_visualization.png)

## Methodology
### Model Architectures
1. **LSTM Network**
   - 256 LSTM units
   - Dropout and Batch Normalization
   - Test Accuracy: 96.4%

2. **GRU Network**
   - 256 GRU units
   - Similar regularization to LSTM
   - Test Accuracy: 95.8%

3. **Deep Neural Network**
   - 5 hidden layers (2548-5096 units)
   - Progressive dropout regularization
   - Test Accuracy: 94.2%

### Training Process
- Adam optimizer with exponential learning rate decay
- Early stopping with model checkpointing
- Class-balanced training through stratified sampling

## Results
### Performance Comparison
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| LSTM  | 96.4%    | 0.96      | 0.96   | 0.96     |
| GRU   | 95.8%    | 0.96      | 0.96   | 0.96     |
| DNN   | 94.2%    | 0.94      | 0.94   | 0.94     |

### Confusion Matrices
![Model Confusion Matrices](images/confusion_matrices.png)

## Installation
```bash
git clone https://github.com/yourusername/brain-emotion-analysis.git
cd brain-emotion-analysis

# Install requirements
pip install -r requirements.txt

# Required libraries
numpy==1.23.5
pandas==1.5.3
tensorflow==2.12.0
scikit-learn==1.2.2
matplotlib==3.7.1
seaborn==0.12.2
## Video Demonstration
**Project Walkthrough Video:**  
[![Watch Video][(https://img.shields.io/badge/Google_Drive-Video_Link-blue?logo=google-drive&style=for-the-badge)](YOUR_GOOGLE_DRIVE_LINK_HERE)
](https://drive.google.com/drive/folders/1jwawQjn5kCHdAOiI7LV0LVTt8hWTcsHd?usp=drive_link)
**Direct Link:**  
[`https://drive.google.com/file/d/YOUR_VIDEO_ID/view?usp=sharing`](https://drive.google.com/drive/folders/1jwawQjn5kCHdAOiI7LV0LVTt8hWTcsHd?usp=drive_link)
