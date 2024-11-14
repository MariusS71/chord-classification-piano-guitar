# Chord Classification for Piano and Guitar 🎹🎸

This project focuses on predicting the type of musical chord (**Major** or **Minor**) from audio recordings of piano and guitar chords using supervised machine learning algorithms.

## Project Overview
- **Objective**: Classify audio recordings as major or minor chords using frequency analysis and machine learning.
- **Dataset**: Kaggle dataset with **859 .wav files** (502 major chords, 357 minor chords).
- **Technologies Used**: Python, scikit-learn, scipy, numpy.

## Methodology
1. **Musical Theory Recap**:
   - Understanding musical scales and chord structures to differentiate major and minor chords.
   - Chords consist of multiple notes played simultaneously, creating harmonic frequencies.

2. **Data Preprocessing**:
   - Applied **Fourier Transform** to convert audio signals from time domain to frequency domain.
   - Extracted harmonic peaks using the `find_peaks` method from `scipy`.
   - Analyzed harmonic intervals to differentiate between major and minor chords based on their unique frequency distributions.

3. **Feature Engineering**:
   - Calculated frequency intervals between harmonic peaks.
   - Selected significant intervals for model training (e.g., Interval 1, Interval 2, Interval 3).
   - Converted chord type labels to binary (1 for Major, 0 for Minor).

4. **Machine Learning Models**:
   - Evaluated multiple classifiers, including:
     - **Random Forest**
     - **K-Nearest Neighbors (KNN)**
     - **Decision Tree**
     - **Gradient Boosting Classifier**
   - Split dataset into **70% training** and **30% testing**.

## Key Features
- Extracts harmonic frequencies and intervals from audio recordings.
- Implements supervised learning algorithms to classify chords with high accuracy.
- Achieved up to **93% accuracy** using Gradient Boosting Classifier.

## Results
- **Gradient Boosting Classifier** achieved the highest accuracy (93%) in distinguishing major and minor chords.
- Analyzing harmonic intervals provided significant insights into chord differentiation.

## Conclusion
The project demonstrates the ability to classify chords using frequency analysis and machine learning techniques. Future improvements could involve expanding the dataset and exploring deep learning models for more complex audio analysis.
