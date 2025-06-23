# audio_genre_classification_lstm

# 🎵 GTZAN Music Genre Classification using LSTM Variants

This project implements and compares deep learning models — **LSTM**, **Residual LSTM (ResLSTM)**, and **Convolutional LSTM (ConvLSTM)** — to classify music genres using the **GTZAN dataset**.

## 📁 Dataset
- **GTZAN Genre Collection**: A popular benchmark dataset consisting of 1,000 audio tracks (30 seconds each) across 10 genres.
- Genres include: *blues, classical, country, disco, hiphop, jazz, metal, pop, reggae, rock*.

## 🧠 Models
We explored three temporal deep learning architectures:
- **LSTM**: Baseline model using sequential learning from audio features
- **ResLSTM**: Adds residual connections to improve gradient flow and performance
- **ConvLSTM**: Incorporates spatial-temporal dependencies using convolutional operations

## 🔧 Features & Preprocessing
- Extracted **MFCC (Mel-Frequency Cepstral Coefficients)** from each audio file
- Normalized features and split dataset into train/validation/test sets
- Reshaped features to fit the expected input shape of each model variant

## 📊 Evaluation Metrics
- **Accuracy**
- **Confusion Matrix**
- **Training/Validation Loss Curves**

## 🧪 Results
- ResLSTM outperforms ConvLSTM & LSTM in overall accuracy, recall, precision, and f1-score across all classes. ResLSTM also minimize the overfitting
- Disco and reggae are the most vulnerable genre to predict from all models (most missclassified happened in these genres)

*(See detailed results in the notebook)*


## 🚀 How to Run
1. Clone this repo
2. Run the notebook which contains preprocessing to model training

## 📌 Future Work
- Use ResLSTM as base model
- Try data augmentation Especially for weak classes like country, disco, hiphop
- Add batch normalization and residual connectionn. May further boost ConvLSTM performance
- Explore Mel spectrogram input instead of MFCC. CNN-based models may learn better from image-like inputs

## 📬 Contact
Feel free to reach out if you want to collaborate or ask questions!

