# 🧠 Parkinson’s Disease Early Detection via MRI & Deep Learning

**parkinson‑s‑diagnosis** proposes a computer-aided diagnosis tool using MRI to detect Parkinson’s disease (PD) with a CNN-based pipeline :contentReference[oaicite:1]{index=1}.

---

## 🔬 Overview

Parkinson’s disease affects over 6 million individuals worldwide. This project aims to reduce diagnostic variability and time by automating PD detection from brain MRI scans using deep learning :contentReference[oaicite:2]{index=2}.

---

## 🚀 Pipeline

1. **Image Enhancement**  
   - Convert to YUV; denoise (Gaussian blur); apply CLAHE to the luminance channel; revert to RGB :contentReference[oaicite:3]{index=3}.

2. **First Stage – ROI Extraction**  
   - A custom CNN filters MRI slices to identify the Substantia Nigra (SN) region, critical for Parkinson’s classification :contentReference[oaicite:4]{index=4}.

3. **Final Stage – Classification**  
   - A modified AlexNet (6 convolutional layers) with sigmoid output classifies SN region images as PD or control :contentReference[oaicite:5]{index=5}.

---
⚙️ Requirements

- Python 3.x  
- TensorFlow / Keras  
- OpenCV, NumPy, Matplotlib, scikit‑image, etc.  
- GPU recommended for training


