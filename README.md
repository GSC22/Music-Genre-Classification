🎵 Music Genre Classification using Log-Mel Spectrograms and Deep Learning

This repository presents an end-to-end Music Genre Classification system built using audio signal processing and deep learning techniques. The core idea of this project is to transform raw audio signals into Log-Mel Spectrogram representations, which closely model human auditory perception, and use these representations to train a neural network capable of accurately identifying music genres.

Unlike traditional approaches that operate directly on raw waveforms, this project leverages time–frequency domain analysis to extract meaningful patterns from audio. The Log-Mel spectrogram acts as a visual representation of sound, enabling convolutional neural networks to learn discriminative features for genre recognition.

📖 Project Overview

Music genre classification is a fundamental problem in Audio AI and Music Information Retrieval (MIR). The objective is to automatically categorize audio tracks into predefined genres such as:

Blues, Classical, Country, Disco, Hip-hop, Jazz, Metal, Pop, Reggae, Rock

This project demonstrates how signal processing + deep learning can be combined to solve real-world audio classification tasks.

🧠 Why Log-Mel Spectrogram?

Human ears do not perceive frequencies linearly. Lower frequencies are perceived with more detail compared to higher frequencies. The Mel scale models this perception, and applying a logarithmic transformation to the amplitude further aligns with how humans perceive loudness.

Therefore, Log-Mel spectrograms:

Preserve important audio characteristics

Reduce dynamic range of signals

Highlight meaningful frequency patterns

Provide an image-like representation ideal for CNN models

This makes Log-Mel features a standard choice in:

Speech Recognition

Music Analysis

Sound Event Detection

Audio Classification systems

⚙️ Methodology

1. Audio Preprocessing

Audio files are loaded and resampled

Noise and silence handled

Signals divided into short time frames


2. Feature Extraction

Short Time Fourier Transform (STFT)

Conversion to Mel scale

Log transformation to obtain Log-Mel spectrogram

Spectrogram visualization for analysis


3. Model Training

Spectrograms used as input to a deep learning model

Model learns time-frequency patterns unique to each genre

Training and validation performed on labeled dataset


4. Prediction

New audio files converted to Log-Mel spectrogram

Model predicts the corresponding music genre



🛠️ Technologies Used

Python

Librosa – Audio processing and feature extraction

NumPy & Matplotlib – Data handling and visualization

TensorFlow / Keras – Deep learning model


🎯 Learning Outcomes

This project helps in understanding:

Fundamentals of Audio Signal Processing

Time–frequency representation of sound

Mel scale and human auditory perception

Feature engineering for audio AI

Applying deep learning to non-image data


📌 Conclusion

This project highlights how converting audio into perceptually meaningful representations such as Log-Mel spectrograms allows deep learning models to effectively perform music genre classification. It serves as a strong foundation for further exploration in Audio AI, Music Information Retrieval, and Deep Learning for Sound.
