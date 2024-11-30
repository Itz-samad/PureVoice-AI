# PureVoice AI

**PureVoice AI** is a real-time noise cleansing solution designed to enhance the quality of calls by effectively removing background noise. It leverages a personalized approach to noise cancellation by recording the user's voice for 30 seconds and training a noise suppression model tailored to the user's unique audio characteristics.

## Features

- **Personalized Voice Capture**: Records 30 seconds of user audio to adapt the noise suppression system for better accuracy.
- **Advanced Noise Cleansing**: Utilizes spectral gating and bandpass filtering to eliminate background noise effectively.
- **Real-Time Processing**: Performs live noise suppression and voice recognition for seamless call experiences.
- **Feature Extraction**: Employs MFCC (Mel-Frequency Cepstral Coefficients) for audio preprocessing.
- **Customizable Neural Network**: Trains a TensorFlow/Keras-based model to distinguish voice from noise.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/purevoice-ai.git
   cd purevoice-ai

pip install -r requirements.txt



## Usage

1. Record Your Voice
Run the script to record 30 seconds of your voice:
run cell record_audio()
This will save your recording in the recordings/ directory.

2. Train the Neural Network
Train a custom model for voice recognition and noise suppression:
run cell build_model()

3. Real-Time Noise Suppression
Start real-time processing for noise-free calls:
run cell real_time_processing()

## File Structure
record_audio.py: Script for recording 30 seconds of audio.
feature_extraction.py: Extracts MFCC features from audio files.
train_model.py: Defines and trains the neural network model.
real_time_processing.py: Implements live noise suppression and voice recognition.
utils/: Contains helper functions for audio preprocessing and filtering.

## Requirements
Python 3.7 or higher
TensorFlow
NumPy
Librosa
PyAudio
SciPy
SoundFile



## How It Works
Voice Recording: Captures a personalized audio sample to fine-tune noise suppression.
Feature Extraction: Extracts MFCC features from audio to train the model.
Model Training: Builds a CNN-LSTM hybrid model for effective noise cancellation.
Real-Time Application: Uses trained models to cleanse audio during live calls.

## Contributing
We welcome contributions! Feel free to open issues or submit pull requests.

## License
This project is licensed under the MIT License. See LICENSE for details.

Developed with ❤️ by Abdulsamad and contributors.
Let me know if you'd like to tweak any section or add more details!