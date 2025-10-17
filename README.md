# EEG-Hybrid-Decoder
Implementation and performance optimization of EEG signal multi-class decoding algorithms based on hybrid deep learning models (CNN, RNN, Transformer).

基于混合深度模型的EEG信号多分类解码算法研究  

**Author:** mushRoom, Yoyo Lee  
**Institution:** Southeast University · School of Artificial Intelligence, School of Software Engineering 

---

## 1. Background
Brain–Computer Interface (BCI) serves as the core technology connecting the human brain to external devices, with non-invasive electroencephalography (EEG) emerging as the mainstream research direction due to its high safety and low cost.  
However, EEG signals exhibit characteristics such as high noise levels, low signal-to-noise ratio, and strong non-stationarity, making it challenging for traditional machine learning methods to effectively extract their deep features.  
This study aims to develop a multi-class decoding algorithm for EEG signals based on a hybrid deep learning model. By integrating the spatial feature extraction capabilities of convolutional neural networks (CNNs) with the temporal modeling capabilities of recurrent neural networks (RNNs) or Transformers, the algorithm achieves higher accuracy and robustness in EEG signal classification.

---

## 2. Objectives
- Construct hybrid deep neural network architectures to jointly model the spatial and temporal features of EEG signals;  
- Reproduce and validate models on various open-source EEG datasets (e.g., BCI Competition IV);  
- Optimize network structures and hyperparameter settings to enhance classification accuracy on validation sets;  
- Explore transfer learning strategies under small-sample conditions to improve cross-subject generalization performance.

---

## 3. Methodology
3.1 Model Structure  
- **CNN Module**: Extracts spatial domain features to capture spatial correlations between signals from different brain regions.  
- **RNN/Transformer Module**: Captures temporal dynamic features of EEG signals.  
- **Fusion Layer**: Performs spatio-temporal feature fusion to enable multi-class output prediction.

### 3.2 Implementation and Framework
- Deep learning framework: **PyTorch 2.x**
- Data processing: **MNE, NumPy**
- Model training: Cross-validation + Adam optimizer + Dynamic learning rate adjustment
- Visualization tools: **Matplotlib, TensorBoard**

### 3.3 Datasets
- BCI Competition IV 2a
- Self-built small-sample EEG dataset (usable for model training and validation)

---

## 4. Experiments & Results
| Model Architecture | Dataset | Classification Task | Accuracy (Validation) | Notes |
|-----------|----------|------------|----------------------|------|
||||||
||||||
||||||

---

## 5. Current Progress
- [x] Read domestic and international papers and reviews on EEG–BCI  
- [x] Complete PyTorch implementation of classic CNN/RNN models  
- [x] Conduct model training and parameter tuning to improve validation accuracy  
- [ ] Implement Transformer fusion module  
- [ ] Complete model performance comparison and visualization analysis  

---

## 6. Project Structure
```
EEG-Hybrid-Decoder/
│
├── data/ # EEG data and preprocessing scripts
├── models/ # Model architecture definitions (CNN, RNN, Transformer)
├── utils/ # Utility functions, e.g., feature extraction, plotting
├── experiments/ # Experiment configurations and results
├── main.py # Main training and testing entry point
├── requirements.txt
└── README.md
```

---

## 7. References
- Chen et al., *Brain–Computer Interfaces in 2023–2024*, Brain-X, 2025.  
- Lawhern et al., Journal of Neural Engineering, IOP Publishing, 2018.  
- Ding et al., Nature Communications, Nature Portfolio, 2025.
---

## 8. Contact
若您对本项目感兴趣或希望交流相关研究，欢迎联系：  
**yo66666666yo@gmail.com**  
或在GitHub上提交Issue与Pull Request。

---

> *This repository aims to promote open research and reproducibility in EEG decoding and hybrid deep learning.*  
> *本项目旨在推动EEG解码与混合深度学习的开源科研与可复现研究。*
