# Speech_Recognition_Group-14

Toronto emotional speech set (TESS)

Dataset : kaggle datasets download -d ejlok1/toronto-emotional-speech-set-tess

This dataset contains 2800 audio recordings of 200 target words spoken in the phrase, each portraying seven emotions: anger, disgust, fear, happiness, pleasant surprise, sadness, and neutral. The recordings are stored in WAV format, organized by actress and emotion.

Key Analyses:
- **Emotion Recognition**: Ideal for training models to classify emotions based on speech using features like pitch and tone.
- **Age Comparison**: Allows for studying how age affects emotional expression in speech.
- **Acoustic Features**: Analysis of pitch, intensity, and speech rate across different emotions.
- **HCI Applications**: Useful for improving voice-driven emotion-sensitive interfaces like virtual assistants.
- **Speaker-Dependent/Independent Models**: Enables model training both specific to and generalized across speakers.

This dataset offers a structured way to explore emotional and age-related variations in speech, benefiting fields like emotion recognition and human-computer interaction.

Project Report: Toronto Emotional Speech Set (TESS)
1. Introduction
The Toronto Emotional Speech Set (TESS) is a dataset designed to study the emotional content in speech. It consists of audio recordings of two actresses speaking a set of 200 target words in seven different emotions: anger, disgust, fear, happiness, pleasant surprise, sadness, and neutral. This dataset is valuable for various applications, such as emotion recognition systems, affective computing, and improving human-computer interaction through emotional speech detection.

The dataset was sourced from Kaggle, and it provides high-quality, labeled audio recordings that can be used to train machine learning models for emotion detection from speech.

2. Objectives
The main objectives of this project are:

To preprocess and explore the TESS dataset.
To apply machine learning techniques for emotion classification based on speech features.
To evaluate the performance of the model in recognizing different emotional states.
3. Dataset Description
The Toronto Emotional Speech Set (TESS) consists of:

Actors: Two female speakers (aged 26 and 64) recording speech.
Emotions: Seven emotions expressed through speech (anger, disgust, fear, happiness, pleasant surprise, sadness, neutral).
Target Words: 200 common words are spoken in each emotion.
File Format: Audio files are in .wav format.
The dataset is freely available on Kaggle and can be downloaded from Kaggle's TESS page.

4. Data Preprocessing
Before analyzing the data, the following preprocessing steps were performed:

Loading and Normalizing Audio: The .wav files were loaded and normalized to ensure that the audio signals have consistent intensity across all recordings.
Feature Extraction: Key features such as Mel-Frequency Cepstral Coefficients (MFCCs), pitch, spectral contrast, and chroma were extracted from the audio files. These features are known to capture essential aspects of speech and are widely used in speech and audio processing.
5. Model and Techniques
To recognize emotions from the speech data, machine learning algorithms were applied:

Feature Selection: MFCC features were selected for their strong correlation with emotional states in speech.
Model Selection: Several classifiers were evaluated for performance, including:
Support Vector Machine (SVM): SVM is known for its robustness in small datasets and high-dimensional data.
Random Forest: An ensemble method that builds multiple decision trees and averages them to improve prediction accuracy.
Convolutional Neural Networks (CNN): CNNs were applied to spectrograms generated from the audio files to leverage deep learning for emotion classification.
6. Results and Evaluation
After training and testing the models, the following results were obtained:

SVM showed high accuracy for detecting emotional states based on MFCC features, particularly excelling in detecting neutral and happy emotions.
Random Forest performed well but showed some overlap between similar emotions like fear and surprise.
CNN models using spectrograms provided the best results, with high precision and recall across all emotional categories.
Accuracy scores were evaluated using a confusion matrix and performance metrics such as precision, recall, and F1-score.

7. Insights and Recommendations
Key insights from this project include:

Neutral vs. Emotional Speech: Neutral speech was easily distinguishable from emotional speech, which aligns with previous research in emotion detection.
Overlap in Emotions: Some emotions, such as fear and surprise, were harder to distinguish due to the similarity in their vocal expression. Further work could involve using more sophisticated deep learning architectures to improve the separation between similar emotions.
Potential Applications: This dataset could be used for creating emotion-aware systems in virtual assistants, automated customer service, and interactive AI systems that adapt to human emotions in real time.
8. Conclusion
The TESS dataset provides a robust foundation for speech-based emotion recognition. By applying feature extraction techniques and machine learning models, this project successfully classified emotions from speech with promising results. Future work could involve using more advanced deep learning models or applying transfer learning techniques to improve the model's generalizability.
