# Emo_Conversational_AI
Conversational AI can express emotions and mimic the nuances of any person's voice as well as emotional characteristics.

## Outline of the project

### Task 1: Transcription of the audio files it can be live-streaming audio or pre-recorded audio files.

I am using the Ctranslate2 library implementation of the whisper model to tackle the latency and for real-time audio transcription I using overlapping batch processing this solves two problems it creates a sense of real-time audio transcription by outputting the transcription in 3-second batches and at the same time does not lose context because of the overlapping of the audio chucks helps in maintaining the context of transcription.

### Dependencies require for this task:
Python 3.8 or greater

portaudio

librosa 

soundfile

av==11.*

ctranslate2>=4.0,<5

huggingface_hub>=0.13

tokenizers>=0.13,<0.16

onnxruntime>=1.14,<2

torch>=2

torchaudio>=2

faster-whisper==1.0.0

transformers

pandas

setuptools>=65

nltk





