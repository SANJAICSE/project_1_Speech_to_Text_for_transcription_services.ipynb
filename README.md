# project_1_Speech_to_Text_for_transcription_services.ipynb
✅ Module 1: Setup
Installs libraries required for speech processing and transcription:

kaggle, transformers, torchaudio, librosa, noisereduce, openai-whisper, datasets, jiwer

📁 Module 2: Data Upload & Cleaning
Uses Google Colab's file uploader to import audio datasets (.tar.gz)

Audio Preprocessing:

Loads .wav file using librosa

Trims silence (librosa.effects.trim)

Normalizes audio (librosa.util.normalize)

Plots waveform

📊 Module 3: Audio Analysis
Computes Spectrogram using Short-Time Fourier Transform (STFT)

Visualizes the spectrogram with dB scaling to inspect signal quality

📈 Module 4: Evaluation – Word Error Rate (WER)
Uses the jiwer package to calculate Word Error Rate between actual and predicted transcripts

Example:

python
Copy
Edit
actual = "please call me back"
predicted = "please coll me back"
wer_score = wer(actual, predicted)
WERs are plotted as a bar chart to visualize performance across different test samples.

