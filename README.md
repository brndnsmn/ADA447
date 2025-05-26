# 🧠 Eye Disease Classification with Fastai

This repository contains a deep learning project for classifying **retinal images** into four common eye disease categories using the **Fastai** library and **transfer learning** with ResNet34.

---

## 📂 Dataset

- Dataset Name: `eye-disease-classification`  
- Source: [Kaggle Dataset](https://www.kaggle.com/datasets/gunavenkatdoddi/eye-diseases-classification)
- Format: JPEG/PNG retina images  
- Total Images: 4217  
- Classes:
  - `normal`
  - `diabetic_retinopathy`
  - `cataract`
  - `glaucoma`

---

## 🧪 Model Architecture

- **Backbone:** `resnet34` pretrained on ImageNet
- **Framework:** Fastai (built on PyTorch)
- **Techniques Used:**
  - `DataBlock` API
  - `Presizing + Augmentation`
  - `Transfer Learning` (Freeze → Unfreeze)
  - `Discriminative Learning Rates`
  - `Learning Rate Finder`
  - `Mixed Precision Training`

---

## 📊 Evaluation

- Accuracy: ~91% on validation set
- Confusion Matrix used for class-wise error analysis
- Top losses were visualized using `ClassificationInterpretation`

---

## 🖼️ Gradio Interface (Deployed)

You can try out the model using the Gradio demo hosted on Hugging Face Spaces:  
👉 [Live Demo on Hugging Face Spaces](https://huggingface.co/spaces/your-username/eye-disease-classification)

<img src="demo_screenshot.png" width="500" />

---

## 🚀 How to Run Locally

```bash
git clone https://github.com/your-username/eye-disease-classification.git
cd eye-disease-classification

# Install dependencies
pip install -r requirements.txt

# Run the app
python app.py
