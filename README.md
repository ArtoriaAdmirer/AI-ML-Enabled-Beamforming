# AI-ML-Enabled Beamforming

A machine learning-enabled beamforming solution designed for industrial-grade URLLC (Ultra-Reliable Low-Latency Communication) in 5G/6G Massive MIMO networks.

## 🎯 Project Overview

This project explores the use of Machine Learning (ML) as an enabling technology for industrial-grade URLLC. With ML, physical-layer network operations become **predictive instead of reactive**, resulting in significantly lower computational latency in real-time optimization.

**Focus**: ML-enabled beamforming for 5G/6G Massive MIMO networks. The high-cost, high-latency operation of determining optimal Zero-Forcing (ZF) beamforming weights is transformed into a supervised learning approach, enabling revolutionary solutions that meet the latency demands of future industry standards.

## ⭐ Key Highlights

- **Predictive vs. Reactive Operations**: ML transforms physical-layer operations from reactive to predictive, enabling significantly lower computational latency
- **Real-World Empirical Data**: All models trained and evaluated on empirical data from actual sensors:
  - Measured Rayleigh fading channels
  - 3GPP CDL channel estimation
  - DeepMIMO (OpenCSI) dataset
- **Performance Tradeoff**: Sophisticated models achieve a balanced compromise—sacrificing peak spectral efficiency for **dramatically reduced computational time**, meeting strict URLLC requirements
- **Industry-Grade Solution**: Designed to meet latency and reliability demands of next-generation 5G/6G applications

## 🔄 Development Stages

The project evolves through multiple iterations with increasing sophistication:

| Stage | Model Type | Focus | Characteristics |
|-------|-----------|-------|-----------------|
| **V1-V2** | MLP | Baseline ML approach | Initial exploration of supervised learning for beamforming |
| **V3** | Ridge Regression | Feature engineering | Improved efficiency with engineered features |
| **V4a** | DNN | Balanced optimization | Trade peak efficiency for reduced latency |
| **V4b** | Advanced DNN | Production-ready | Optimized for minimal computational overhead |

## 🔬 Methodology

The research approach:
1. **Maps** the complex relationship between Channel State Information (CSI) and optimal Zero-Forcing beamformers
2. **Learns** beamforming weights using supervised learning from empirical channel data
3. **Replaces** high-latency optimization with efficient low-latency neural network inference
4. **Validates** all models against real-world channel measurements to ensure practical applicability

## 📊 Key Findings

- ✅ Sophisticated ML algorithms effectively learn the mapping between experimental CSI and optimal beamformers
- ✅ Later iterations (V4a/V4b) achieve significant computational speedup while maintaining acceptable spectral efficiency
- ✅ Models trained on empirical data show strong generalization to unseen channel conditions
- ✅ Revolutionary ML-based beamforming solution achieves all latency demands required for future industrial standards

## 🚀 Features

- **Advanced Beamforming Algorithms**: MVDR, Capon's, Delay-and-Sum, Zero-Forcing, and adaptive methods
- **ML Model Portfolio**: MLP, Ridge Regression, and Deep Neural Networks across multiple development stages
- **Signal Processing Pipeline**: Comprehensive array signal processing and analysis tools
- **Adaptive Filtering**: Real-time adaptive filters for optimal beam adjustment
- **Performance Metrics**: Spectral efficiency, latency, and generalization analysis
- **Real-World Validation**: Extensively tested on empirical sensor data and channel measurements
- **Production-Ready**: Optimized models for deployment in latency-critical applications

## 📁 Project Structure

```
AI-ML-Enabled-Beamforming/
├── README.md                          # Main project documentation
├── Notebooks/                         # Jupyter notebooks by development stage
│   ├── V1-V2_MLP/
│   ├── V3_Ridge_Regression/
│   ├── V4a_DNN/
│   └── V4b_Advanced_DNN/
├── datasets/                          # Dataset access guide and links
│   ├── README.md                      # Google Drive link and usage instructions
│   ├── rayleigh_fading/              # Rayleigh channel measurements
│   ├── 3gpp_cdl/                     # 3GPP CDL channel data
│   └── deepmimo_opencsi/             # DeepMIMO dataset files
├── src/                               # Source code and implementations
├── models/                            # Pre-trained ML model files
├── Project Report and Publications/   # Technical reports and research papers
│   ├── project_report/
│   ├── publications/
│   └── supplementary/
├── tests/                             # Unit tests
├── docs/                              # Additional documentation
└── requirements.txt                   # Python dependencies
```

## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- NumPy >= 1.19
- SciPy >= 1.5
- TensorFlow >= 2.4 or PyTorch >= 1.7 (for DNN models)
- scikit-learn >= 0.24
- Jupyter Notebook (for running notebooks)

### Installation

1. **Clone the repository**:
```bash
git clone https://github.com/ArtoriaAdmirer/AI-ML-Enabled-Beamforming.git
cd AI-ML-Enabled-Beamforming
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```

3. **Download datasets**:
   - Visit the [Datasets](./datasets/README.md) folder for Google Drive links
   - Download required datasets and place them in the `datasets/` directory

### Quick Start

1. **Explore notebooks**: Navigate to `Notebooks/` folder to see development stages from V1 to V4b
2. **Review methodology**: Check `Notebooks/` for detailed explanations of each approach
3. **Reproduce results**: Run notebooks in sequential order to understand model progression
4. **Evaluate models**: Use provided evaluation scripts to assess performance metrics

## 📖 Detailed Documentation

- **[Notebooks](./Notebooks/)**: Comprehensive Jupyter notebooks documenting each development stage
- **[Datasets Guide](./datasets/README.md)**: Instructions for accessing and using empirical channel datasets
- **[Project Reports & Publications](./Project%20Report%20and%20Publications/)**: Technical documentation and research papers

## 🧠 Models and Algorithms

### Beamforming Techniques
- **Delay-and-Sum Beamforming**: Baseline reference implementation
- **Zero-Forcing (ZF) Beamforming**: Optimal linear precoding (learning target)
- **MVDR (Minimum Variance Distortionless Response)**: Adaptive classical approach
- **Capon's Method**: Minimum variance spectral estimation
- **Adaptive Beamforming**: Real-time adaptation algorithms

### ML Models Evolution
| Version | Architecture | Training Data | Performance | Use Case |
|---------|-------------|---------------|-------------|----------|
| V1 | Multi-Layer Perceptron | Synthetic/Limited | Baseline | Proof of concept |
| V2 | Enhanced MLP | Expanded dataset | Improved | Initial validation |
| V3 | Ridge Regression | Engineered features | Competitive | Feature-rich approach |
| V4a | DNN (3-4 layers) | Empirical channels | High efficiency | Research |
| V4b | Advanced DNN (optimized) | Real-world data | Production-ready | Deployment |

## 📊 Performance Evaluation

Models are evaluated across multiple dimensions:

- **Spectral Efficiency vs. Latency Tradeoff**: Primary performance metric
- **Real-World Channel Accuracy**: Validation against measured channel data
- **URLLC Compliance**: Latency and reliability guarantees
- **Generalization**: Performance on unseen channel conditions
- **Computational Efficiency**: Inference time and resource requirements

## 📚 Datasets

All models are trained and evaluated using empirical data:

- **Rayleigh Fading Channels**: Real measured channel impulse responses
- **3GPP CDL**: Industry-standard 3GPP Clustered Delay Line models
- **DeepMIMO (OpenCSI)**: Large-scale MIMO channel dataset for deep learning

👉 **[Download Datasets](./datasets/README.md)**

## 🔗 Notebooks Overview

| Notebook | Focus | Output |
|----------|-------|--------|
| `V1-V2_MLP` | Baseline MLP implementation | Model performance metrics |
| `V3_Ridge_Regression` | Engineered features approach | Feature importance analysis |
| `V4a_DNN` | Deep neural network development | Optimized model checkpoint |
| `V4b_Advanced_DNN` | Production optimization | Deployment-ready model |

## 🤝 Contributing

Contributions are welcome! Areas for contribution:
- Additional beamforming algorithm implementations
- Optimization of model architectures
- Extended dataset validation
- Performance benchmarking
- Documentation improvements

Please submit a pull request or open an issue to discuss potential improvements.

## 📄 License

[Specify your license here]

## 📚 References & Further Reading

[Add key papers, standards, and resources:
- 3GPP Technical Specifications
- DeepMIMO dataset papers
- Machine learning for signal processing research]

## 👤 Contact & Support

For questions, issues, or inquiries:
- Open an issue on this repository
- Contact the repository maintainer

---

## 🌟 Project Status

- ✅ Core ML models implemented and validated
- ✅ Datasets organized and linked
- ✅ Notebooks and documentation in place
- 🔄 Ready for community contributions
- 🎯 Continuing optimization and benchmarking

**Last Updated**: July 2026

---

**Note**: This project represents cutting-edge research in ML-enabled physical-layer optimization for 5G/6G networks, designed to meet the latency and reliability demands of industrial URLLC applications.
