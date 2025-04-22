# 🎤 Speech Emotion Recognition – Baseline Model

This repository contains a baseline machine learning pipeline for **speech emotion recognition** using audio data. The model leverages the **RAVDESS dataset** and uses traditional signal processing techniques combined with a **Support Vector Machine (SVM)** classifier for predicting emotional states from speech.

---

## 🎯 Objective

To classify emotional states such as `happy`, `sad`, `angry`, `calm`, `fearful`, etc., based on extracted features from audio clips.

---

## 🧠 Feature Extraction

The script extracts a combination of audio features using the `librosa` library:

- **MFCCs (Mel Frequency Cepstral Coefficients)**
- **Chroma Frequencies**
- **Mel Spectrogram**
- **Spectral Contrast**
- **Tonnetz Features**

These features are concatenated into a single vector for each audio clip.

---

## 🛠️ Model Pipeline

1. **Audio Preprocessing**
   - Reads audio from `.wav` files.
   - Parses file names to extract emotion labels.

2. **Feature Extraction**
   - Applies `librosa` to extract spectral and temporal features.

3. **Classification**
   - Uses **Support Vector Machine (SVM)** via `scikit-learn`.
   - Applies **GridSearchCV** for hyperparameter tuning.

4. **Evaluation**
   - Prints accuracy, confusion matrix, and classification report.

---

## 📂 Project Structure

```
.
├── baseline_model.py       # Main training & evaluation script
├── README.md               # Project overview and usage
├── audio/                  # Directory where RAVDESS .wav files are extracted
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/speech-emotion-baseline.git
cd speech-emotion-baseline
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Download the RAVDESS dataset

- Download the `.zip` or audio files from [RAVDESS official site](https://zenodo.org/record/1188976).
- Unzip the files into an `audio/` folder in the project root.

### 4. Run the model

```bash
python baseline_model.py
```

---

## 📊 Output

After training, the script will display:
- Accuracy score
- Confusion matrix (visualized with seaborn)
- Classification report with precision, recall, and F1-score

---

## 📚 Requirements

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `librosa`
- `scikit-learn`

---

## 👏 Acknowledgements

- Based on the [RAVDESS Dataset](https://zenodo.org/record/1188976)
- Built using `librosa`, `sklearn`, and `matplotlib`

---

