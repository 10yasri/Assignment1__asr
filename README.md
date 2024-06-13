LibriSpeech ASR Evaluation
This project uses the pre-trained Wav2Vec2 model from Facebook to transcribe audio files from the LibriSpeech dataset and evaluate the transcription accuracy using the Character Error Rate (CER) metric.
Table of Contents:
Installation
Usage
Project Structure
Example Output
Contributing
License

Installation Prerequisites:
Ensure you have the following installed:

Python 3.6 or later
Pip (Python package installer)

Clone the Repository

Create a Virtual Environment

It's recommended to use a virtual environment to manage dependencies:

Install Dependencies
pip install -r requirements.txt

Additional Installations
Install the required libraries manually if not listed in requirements.txt:
pip install torch torchaudio librosa transformers jiwer

Usage:
Load and Transcribe Audio Files

Make sure to update the main_directory variable in the script with the path to your LibriSpeech dataset.

Script Overview
The main script performs the following steps:

Load audio files and corresponding transcriptions from the LibriSpeech dataset.
Use the Wav2Vec2 model to transcribe the audio files.
Calculate and print the Character Error Rate (CER) for the transcriptions.
Project Structure
transcribe.py: Main script to load data, transcribe audio, and calculate CER.
requirements.txt: List of Python dependencies.
Example Output

CER for dev_clean: 0.000480581759616936
CER for test-clean: 0.0015161220170302819
CER for test-other: 0.0020595485028878967
{'dev_clean': 0.000480581759616936, 'test-clean': 0.0015161220170302819, 'test-other': 0.0020595485028878967}


License
This project is licensed under the MIT License. See the LICENSE file for details.


