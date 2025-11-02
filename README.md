

![Alt text](https://github.com/heyawen256-png/fracture_recongnize_predict/blob/main/result.png)

# Identification of Natural Fractures in Shale Reservoirs Using a Multimodal Neural Network: A Case Study of the Chang 7 Shale Formation in the Ordos Basin

## 📌 Project Overview
This repository contains a **multi-modal deep neural network** for predicting natural fracture properties—**occurrence, dip angle, and aperture**—in shale oil reservoirs. The model integrates **conventional well logs** and **borehole imaging data** to provide accurate and efficient fracture characterization, reducing reliance on specialized logging tools and supporting geological and engineering evaluations.

## 🧠 Model Architecture
We developed a coupled **CNN + DNN** architecture:
- **CNN branch**: Extracts spatial features from borehole imaging logs
- **DNN branch**: Captures nonlinear relationships from conventional well logs
- **Multi-modal fusion**: Combines features from both branches for final prediction

## 📊 Performance
| Metric | Training Accuracy | Testing Accuracy |
|--------|-------------------|------------------|
| Dip Angle | 98.82% | 98.82% |
| Aperture | 95.97% | 95.91% |

- **Dip Angle**: Predicted values concentrated between **65°–80°**, with deviation < **0.48°**
- **Aperture**: Predicted values mainly within **0.5–4.5 cm**, deviation < **0.21 cm** (excluding outliers)

## 🛠 Installation & Usage

### Requirements
- Python 3.8+
- TensorFlow 2.x
- PyTorch 1.9+
- NumPy, Pandas, Scikit-learn
- Matplotlib, Seaborn
- OpenCV

### Install Dependencies
```bash
pip install tensorflow torch numpy pandas scikit-learn matplotlib seaborn opencv-python
