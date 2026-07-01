# 🎥 Video Transformer for Deepfake Detection

A deep learning framework for detecting **deepfake videos** using a combination of **Convolutional Neural Networks (CNNs)** and **Transformer architectures**. The model extracts spatial features from individual video frames and learns temporal relationships across frames to accurately classify videos as **Real** or **Deepfake**.

---

## 📌 Overview

Deepfake generation techniques have become increasingly sophisticated, making automated detection an important research problem. This project leverages CNNs for feature extraction and Transformer-based attention mechanisms for temporal modeling, enabling robust video-level deepfake detection.

---

## ✨ Features

- 🎯 Deepfake video classification
- 🧠 CNN-based spatial feature extraction
- 🔄 Transformer-based temporal feature learning
- 📊 Training and evaluation pipeline
- 📈 Feature map visualization
- 🔍 Dataset verification utilities
- 🧩 Modular and extensible project structure

---

## 📂 Project Structure

```text
Video-transformer-for-deepfake-detection/
│
├── attention_lib/              # Attention modules
├── data/                       # Data processing utilities
├── dataset/                    # Dataset loader
├── network/                    # Model architectures
├── tfe/                        # Transformer Feature Encoder
├── visualize/                  # Visualization utilities
│
├── train_CNN.py                # Model training script
├── test_time.py                # Model testing/inference
├── verify_dataset.py           # Dataset verification
├── visualize_feat_map.py       # Feature map visualization
├── visualize_rel.py            # Attention relationship visualization
├── loss_fn.py                  # Loss functions
├── requirements.txt            # Project dependencies
└── README.md
```

---

## 🧠 Methodology

The detection pipeline consists of the following stages:

1. Load video dataset.
2. Extract representative video frames.
3. Process frames using a CNN backbone.
4. Learn temporal dependencies using Transformer layers.
5. Classify the video as **Real** or **Deepfake**.

```text
Video
   │
   ▼
Frame Extraction
   │
   ▼
CNN Feature Extraction
   │
   ▼
Transformer Encoder
   │
   ▼
Classification Layer
   │
   ▼
Real / Deepfake
```

---

## 🚀 Installation

### Clone the repository

```bash
git clone https://github.com/akhilu24/Video-transformer-for-deepfake-detection.git
cd Video-transformer-for-deepfake-detection
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## 📦 Requirements

- Python 3.9+
- PyTorch
- Torchvision
- NumPy
- OpenCV
- Matplotlib

---

## 📊 Dataset

Place your dataset inside the `dataset/` directory.

```text
dataset/
├── train/
├── validation/
└── test/
```

Supported datasets include:

- FaceForensics++
- Celeb-DF
- DFDC
- Custom video datasets

---

## ▶️ Training

```bash
python train_CNN.py
```

---

## 🧪 Testing

```bash
python test_time.py
```

---

## 📈 Visualization

Feature maps:

```bash
python visualize_feat_map.py
```

Attention relationships:

```bash
python visualize_rel.py
```

---

## 📋 Results

Typical evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

---

## 🔮 Future Improvements

- Vision Transformer (ViT) backbone
- EfficientNet-based feature extraction
- Real-time webcam inference
- Streamlit web application
- Model quantization for deployment
- ONNX/TensorRT optimization
- Multi-modal deepfake detection

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push your branch.
5. Open a Pull Request.

---

## 📄 License

This project is intended for educational and research purposes.
