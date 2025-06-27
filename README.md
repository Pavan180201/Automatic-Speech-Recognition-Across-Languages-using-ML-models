# 🗣️ Multilingual Automatic Speech Recognition using Spoken Wikipedia Corpora

This project explores the application of machine learning techniques to improve **automatic speech recognition (ASR)** across multiple languages using the **Spoken Wikipedia Corpora (SWC)** dataset. It focuses on transcription accuracy, denoising methods, and robust feature selection to build a reliable ASR system.

---

## 📌 Project Highlights

- Used **Random Forest Classifier** to predict languages from speech features.
- Applied advanced **denoising techniques**: spectral subtraction, Wiener filtering, and spectral gating.
- Extracted speech features: **MFCC**, **Chroma**, and **Spectral Contrast**.
- Compared model performance on original vs. denoised datasets.
- Achieved **0.77 accuracy and F1-score** after denoising and feature engineering.

---

## 📂 Dataset

**Spoken Wikipedia Corpora (SWC)** — a multilingual dataset with aligned audio-text pairs in:
- **English**
- **German**
- **Dutch**

Real-world conditions with background noise make it ideal for evaluating noise-robust ASR models.

---

## ⚙️ Techniques Used

- **Data Preprocessing**: Audio segmentation, silence trimming, normalization.
- **Noise Reduction**: Spectral Subtraction, Spectral Gating, Wiener Filtering.
- **Feature Engineering**:
  - `13 MFCCs`
  - `12 Chroma Features`
  - `7 Spectral Contrast Values`
- **Statistical Tests**: Chi-Square test for feature selection.
- **Dimensionality Reduction**: PCA retaining 95% variance.
- **Modeling**: Random Forest with Grid Search for hyperparameter tuning.

---

## 📊 Results

| Dataset       | Accuracy | F1-Score |
|---------------|----------|----------|
| Original      | 0.75     | 0.75     |
| After Denoising | **0.77** | **0.77** |

✅ A **paired t-test** confirmed the improvement is statistically significant (p = 0.0005).

---

## 📈 Future Scope

- Explore deep learning models (e.g., CNNs, RNNs) for ASR.
- Integrate real-time multilingual transcription.
- Apply more sophisticated denoising algorithms.

---

## 🧠 Author

**Pavan Kumar Chintala**   
Email: *chintalap014@gmail.com*

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
