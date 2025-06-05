
# 🧠 Emotion Detection Using EEG-Based Brain-Computer Interface

This repository presents a machine learning-based approach for detecting human emotions using EEG signals obtained from a MUSE headband. The project was undertaken as part of a collaborative undergraduate research effort and demonstrates the use of Gated Recurrent Units (GRUs) for time-series classification in brain-computer interface (BCI) applications.

> ⚠️ Note: This paper was not officially published in any journal or conference.

## 🎯 Objective

The core aim of this work was to explore emotion detection through non-verbal EEG data, overcoming the manipulation and limitations of text, speech, or facial expression-based methods. By leveraging EEG signals, the project targeted accurate emotion classification into **positive**, **neutral**, and **negative** states.

## 🧪 Dataset

- **Source:** [Kaggle EEG Brainwave Emotion Dataset](https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions)
- **Device:** MUSE Headband (4 channels: TP9, AF7, AF8, TP10)
- **Data Size:** 30 minutes (2 subjects, 3 minutes per emotion class)
- **Features Used:** FFT, Shannon Entropy, Log-Covariance, Power Spectral Density, etc.
- **Preprocessing:** Feature selection using OneR, Information Gain, Correlation, and others

## 🧠 Model

We used a **Gated Recurrent Unit (GRU)** neural network to model the temporal dependencies in EEG signals:
- 512 GRU units
- Softmax output layer for 3-class classification
- Trained on Google Colab (70% train, 30% test split)
- Optimizer: Adam; Loss: Sparse Categorical Crossentropy

## 📈 Results

| Class     | Precision | Recall | F1-Score |
|-----------|-----------|--------|----------|
| Negative  | 0.97      | 0.98   | 0.98     |
| Neutral   | 1.00      | 0.98   | 0.99     |
| Positive  | 0.96      | 0.97   | 0.96     |
| **Overall Accuracy** |     |        | **97.656%** |

The GRU model outperformed several traditional classifiers (e.g., SVM, Random Forest, Naive Bayes) in terms of accuracy, demonstrating the potential of deep learning in EEG-based emotional analysis.

## 📚 What You Can Learn From This

- EEG-based emotion classification pipeline
- Feature engineering and selection for physiological data
- Deep learning (GRU) for time-dependent signal classification
- How emotion detection can enhance AI-based therapy and human-computer interaction systems

## 🚀 Applications

- AI-driven mental health assistants
- Emotion-aware chatbots
- Neurofeedback and meditation systems
- Cognitive and behavioral research tools

---

## 📝 Citation

If you're referencing or building upon this work in academic or personal projects, please consider citing the authors or linking back to this repository.

