# EEG-Hybrid-Decoder
Implementation and performance optimization of EEG signal multi-class decoding algorithms based on hybrid deep learning models (CNN, RNN, Transformer).

# EEG-Hybrid-Decoder
基于混合深度模型的EEG信号多分类解码算法研究  
**Author:** mushRoom, Yoyo Lee  
**Institution:** Southeast University · School of Artificial Intelligence, School of Software Engineering 

---

## 🧠 1. 研究背景（Background）
脑机接口（Brain–Computer Interface, BCI）是连接人脑与外部设备的核心技术，其中非侵入式脑电图（EEG）因其高安全性和低成本成为主流研究方向。  
然而，EEG信号具有**高噪声、低信噪比和非平稳性强**等特点，传统机器学习方法难以有效提取其深层特征。  
本研究旨在构建一种**基于混合深度模型的EEG信号多分类解码算法**，融合卷积神经网络（CNN）的空间特征提取能力与循环神经网络（RNN）或Transformer的时间建模能力，从而实现更高精度、更鲁棒的EEG信号分类。

---

## ⚙️ 2. 研究目标（Objectives）
- 构建混合深度神经网络结构，实现EEG信号的空间与时间特征联合建模；  
- 对不同开源EEG数据集（如BCI Competition IV等）进行模型复现与验证；  
- 优化网络结构与超参数设置，提高模型在验证集上的分类准确率；  
- 探索小样本条件下的迁移学习策略，提升跨被试泛化性能。

---

## 🧩 3. 方法框架（Methodology）
### 3.1 模型结构
- **CNN 模块**：提取空间域特征，捕捉不同脑区信号间的空间相关性。  
- **RNN/Transformer 模块**：捕捉EEG信号的时间动态特征。  
- **融合层（Fusion Layer）**：进行时空特征融合，实现多类别输出预测。

### 3.2 实现与框架
- 深度学习框架：**PyTorch 2.x**
- 数据处理：**MNE, NumPy, SciPy**
- 模型训练：交叉验证 + Adam优化器 + 学习率动态调整
- 可视化工具：**Matplotlib, TensorBoard**

### 3.3 数据集（Datasets）
- BCI Competition IV 2a（运动想象任务）
- SEED Dataset（情绪识别任务）
- 自建小样本EEG数据（用于验证模型迁移能力）

---

## 📈 4. 实验与结果（Experiments & Results）
| 模型结构 | 数据集 | 分类任务 | 准确率（Validation） | 备注 |
|-----------|----------|------------|----------------------|------|
||||||
||||||
||||||

> ✅ 模型通过结构融合显著提高了多分类任务的稳定性与准确率。

---

## 🔬 5. 当前进展（Current Progress）
- [x] 阅读国内外EEG–BCI相关论文与综述  
- [x] 完成经典CNN/RNN模型的PyTorch复现  
- [x] 进行模型训练与参数调优，提高validation accuracy  
- [ ] 实现Transformer融合模块  
- [ ] 完成模型性能对比与可视化分析  

---

## 🚀 6. 项目结构（Project Structure）
```
EEG-Hybrid-Decoder/
│
├── data/ # EEG 数据与预处理脚本
├── models/ # 模型结构定义（CNN, RNN, Transformer）
├── utils/ # 工具函数，如特征提取、绘图
├── experiments/ # 实验配置与结果
├── main.py # 主训练与测试入口
├── requirements.txt # 依赖包
└── README.md # 项目说明文档
```

---

## 📚 7. 引用与参考文献（References）
- Chen et al., *Brain–Computer Interfaces in 2023–2024*, Brain-X, 2025.  
- Lawhern et al., Journal of Neural Engineering, IOP Publishing, 2018.  
- Ding et al., Nature Communications, Nature Portfolio, 2025.
---

## 📩 8. 联系方式（Contact）
若您对本项目感兴趣或希望交流相关研究，欢迎联系：  
📧 **yo66666666yo@gmail.com**  
或在GitHub上提交Issue与Pull Request。

---

> 🌟 *This repository aims to promote open research and reproducibility in EEG decoding and hybrid deep learning.*  
> *本项目旨在推动EEG解码与混合深度学习的开源科研与可复现研究。*
