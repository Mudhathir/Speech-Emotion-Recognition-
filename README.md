

---

# 🎙️ Speech Emotion Recognition with CNN + BiLSTM

This project implements a deep learning pipeline for recognizing emotions from speech using the **RAVDESS** dataset. It combines **Mel spectrogram-based preprocessing** with a **CNN + BiLSTM architecture** to classify speech into 8 distinct emotional categories.

---

## 📁 Dataset

**RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**  
- Contains high-quality audio clips labeled with 8 emotions: *neutral, calm, happy, sad, angry, fearful, disgust, and surprised*.  
- Balanced across actors and genders for robust training.

---

## 🧠 Model Overview

- **Preprocessing**: Raw audio is converted into **Mel spectrograms**, which highlight the frequency-time structure of speech.
- **Model Architecture**:
  - `CNN` layers for local feature extraction from spectrogram images.
  - `BiLSTM` layers to capture temporal patterns and context.
- **Output**: Softmax classifier to predict one of the 8 emotional states.

---

## 🛠️ Requirements

- Python ≥ 3.8  
- TensorFlow  
- NumPy  
- Librosa  
- Scikit-learn  
- Matplotlib

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. **Preprocess the dataset**:
   - Convert audio clips to Mel spectrograms using Librosa.
2. **Train the model**:
   - Run `nn_final_update.py` to train CNN + BiLSTM on the processed dataset.
3. **Evaluate results**:
   - The model reports accuracy, loss, and classification metrics on a validation set.

---

## 📊 Results

The model demonstrates strong performance in recognizing emotional cues from speech, with notable accuracy improvements due to the combination of CNN feature extraction and BiLSTM temporal modeling.

---

## 💡 Applications

- Emotion-aware virtual assistants  
- Mental health monitoring through voice  
- Intelligent customer service interactions  
- Affective computing in games and education  

---

## 📌 Acknowledgments

- [RAVDESS Dataset](https://zenodo.org/record/1188976)
- Inspired by work in speech-based affective computing and deep learning for audio processing.

---
