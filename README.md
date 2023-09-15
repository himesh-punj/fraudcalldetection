Scam Call Detector v1.2

This Python script is a Scam Call Detector that uses audio analysis and speech recognition to determine the likelihood of a phone call being a scam. It also provides a real-time analysis option for audio input through a microphone. The script includes a graphical user interface (GUI) built using the tkinter library for ease of use.
Prerequisites

Before running the script, make sure you have the required libraries installed. You can install them using pip:

bash

pip install pydub tkinter customtkinter speech_recognition nltk

Additionally, download the NLTK stopwords data by running:

python

nltk.download('stopwords')

Usage

    Select an Audio File:
        Click the "Browse" button to select an audio file (in WAV format) you want to analyze for scam call content.

    Set Pitch and Speed (optional):
        You can adjust the pitch and speed of the audio for analysis. Leave these fields empty or set them to 0 and 1.0, respectively, for default settings.

    Analyze:
        Click the "Analyze" button to analyze the selected audio file. The script will process the audio, transcribe it, and calculate the probability of it being a scam call.

    Start Real-Time Analysis (optional):
        Click the "Start Real-Time Analysis" button to enable real-time audio analysis through your microphone. The script will continuously listen for audio input and provide scam call probability.

    Stop Real-Time Analysis (optional):
        Click the "Stop" button to stop real-time analysis. The final scam call probability for the last segment will be displayed.

Scam Detection Algorithm

The script uses a scam detection algorithm based on the presence of specific scam-related keywords and sentence structures. It calculates the likelihood of a call being a scam based on these factors.
Scam Words and Sentences

The script defines a list of scam words and sentences for scam detection. Scam sentences are used as reference points to identify scam-related content.
Acknowledgments

This script uses the following Python libraries:

    pydub: Audio processing and splitting.
    tkinter: GUI development.
    speech_recognition: Speech recognition and audio analysis.
    nltk: Natural language processing for stopword removal.

Note

This is a basic version (v1.2) of a scam call detector. The accuracy of scam detection may vary, and it is not guaranteed to detect all scam calls accurately.

For more advanced scam call detection, consider using machine learning-based models and more extensive datasets.

Disclaimer: This script is for educational purposes and may not be suitable for real-world scam call detection. Always exercise caution and verify the authenticity of calls and messages from unknown sources.
