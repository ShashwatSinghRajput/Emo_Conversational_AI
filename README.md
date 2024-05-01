# Emo_Conversational_AI
Conversational AI that expresses emotions and mimics human voice nuances and emotional characteristics.

## Outline of the Project

### Task 1: Transcription of Audio Files
Utilizing Ctranslate2 with the Whisper model to address latency in real-time audio transcription. Overlapping batch processing ensures a seamless transcription experience while maintaining context.

Additional testing with WhisperX: [WhisperX GitHub](https://github.com/m-bain/whisperX/tree/main)

#### Dependencies for this task:
- Python 3.8+
- portaudio
- librosa
- soundfile
- av==11.*
- ctranslate2>=4.0,<5
- huggingface_hub>=0.13
- tokenizers>=0.13,<0.16
- onnxruntime>=1.14,<2
- torch>=2
- torchaudio>=2
- faster-whisper==1.0.0
- transformers
- pandas
- setuptools>=65
- nltk

### Installation of Prerequisites

#### PortAudio (audio I/O library)

##### Linux
- Debian/Ubuntu: `sudo apt-get install portaudio19-dev`
- Red Hat/Fedora: `sudo dnf install portaudio-devel`

##### macOS
- Install Homebrew, then: `brew install portaudio`

##### Windows
- Install vcpkg, then: `vcpkg install portaudio`

### Task 2: Interaction with Large Language Models
Testing various large language models to generate responses based on transcribed input.

Models to test:
1. [LLAMA 3](https://github.com/meta-llama/llama3)
2. [LLAMA 2](https://github.com/meta-llama/llama)
3. [GPT-2](https://github.com/openai/gpt-2/tree/master)
4. [FALCON](https://huggingface.co/tiiuae/falcon-40b)
5. [MISTRAL](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2)

#### Dependencies:
- torch
- fairscale
- fire
- sentencepiece
- regex
- requests
- tqdm

### Tools Required
- **wget**: For downloading data.
- **md5sum**: To verify data integrity.

### Task 3: Voice Synthesis
Initial implementation based on [Real-Time Voice Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning), with plans for advanced models in future iterations.

#### Required Dependencies:
- Please create a separate environment due to compatibility issues with older dependencies:
  - ffmpeg
  - PyTorch
  - Pyaudio
  - torchaudio
  - inflect==5.3.0
  - librosa==0.8.1
  - matplotlib==3.5.1
  - numpy==1.20.3
  - Pillow==8.4.0
  - PyQt5==5.15.6
  - scikit-learn==1.0.2
  - scipy==1.7.3
  - sounddevice==0.4.3
  - SoundFile==0.10.3.post1
  - tqdm==4.62.3
  - umap-learn==0.5.2
  - Unidecode==1.3.2
  - urllib3==1.26.7
  - visdom==0.1.8.9
  - webrtcvad==2.0.10

## Adding Streamlit for Web Application Development
To enable web-based interaction, Streamlit will be used for creating intuitive and interactive web interfaces.

### Streamlit Requirements:
- Ensure the server has Python 3.8+ installed.
- Install Streamlit using pip:
- I will require to host this on public network as I can't access the university server on the same network as mine.






