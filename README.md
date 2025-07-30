
# Fog

An advanced research project on robust object classification under various fog intensities and types, based on a multi-scale Transformer model with density-aware attention.

## 🧠 Objective

To develop a high-performance image classifier capable of maintaining strong accuracy even under visually degraded conditions caused by fog.  
The model leverages:
- A cross-scale attention mechanism
- An optimization strategy based on OneCycleLR
- Five types of fog (uniform, gradient, patchy, adaptive, dense)

## 🚀 Key Features

- Realistic fog simulations on CIFAR-10
- Custom architecture based on Vision Transformers
- Class-wise robustness analysis
- Visualization of classification results

## 📦 Technologies Used

- Python 3.10
- PyTorch
- NumPy
- Matplotlib
- Scikit-learn
- OpenCV
- Jupyter Notebook

## 📁 Project Structure

```
.
├── Fog_Density_Aware_Cross_Scale_Transformer_5Types_Fog_Optimizing.ipynb
├── data/
│   └── (CIFAR-10 images simulated with fog)
├── models/
│   └── transformer_fdacst.py
├── utils/
│   └── fog_simulation.py
├── requirements.txt
└── README.md
```

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/oshifils/Fog_Density_Aware_Cross_Scale_Transformer.git
cd Fog_Density_Aware_Cross_Scale_Transformer
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # for Linux/macOS
venv\Scripts\activate     # for Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## 🧪 Running the Notebook

Open the notebook in Jupyter:
```bash
jupyter notebook Fog_Density_Aware_Cross_Scale_Transformer_5Types_Fog_Optimizing.ipynb
```

> ⚠️ Ensure that the fog-augmented CIFAR-10 images are correctly placed in the `./data` directory.

## 📊 Results

| Condition            | Accuracy (%) |
|----------------------|--------------|
| No fog               | 84.4         |
| Light fog            | 81.3         |
| Moderate fog         | 77.5         |
| Dense fog            | 74.2         |
| Extreme fog          | 70.1         |

- **High robustness** for vehicles and animals
- **15.8% improvement** compared to standard Transformers

## 📌 Future Work

- Evaluation on real-world datasets (Dashcam, Foggy Cityscapes)
- Extension to semantic segmentation
- Integration of anomaly detection

## 👤 Author

- **OSHASHA OSHASHA Fiston**  
Researcher in Applied Artificial Intelligence and Distributed Systems  
GitHub: [@oshifils](https://github.com/oshifils)

## 📄 License

This project is released under the **MIT License**.  
You are free to use, modify, and redistribute it with proper attribution.
