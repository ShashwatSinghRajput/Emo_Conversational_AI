# Emo_Conversational_AI
Conversational AI can express emotions and mimic the nuances of any person's voice as well as emotional characteristics.

## Outline of the project

### Task 1: Transcription of the audio files it can be live-streaming audio or pre-recorded audio files.

I am using the Ctranslate2 library implementation of the whisper model to tackle the latency and for real-time audio transcription I using overlapping batch processing this solves two problems it creates a sense of real-time audio transcription by outputting the transcription in 3-second batches and at the same time does not lose context because of the overlapping of the audio chucks helps in maintaining the context of transcription.

I also plan to test WhisperX [https://github.com/m-bain/whisperX/tree/main]

### Dependencies required for this task:
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

## Prerequisites

This project requires `PortAudio`, an audio I/O library that enables low-latency audio processing.

### Installation

#### Linux
- Debian/Ubuntu: `sudo apt-get install portaudio19-dev`
- Red Hat/Fedora: `sudo dnf install portaudio-devel`

#### macOS
- Install Homebrew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- `brew install portaudio`

#### Windows
- Install vcpkg: Follow the instructions at https://github.com/microsoft/vcpkg
- `vcpkg install portaudio`

Please ensure that you have the appropriate development files for `PortAudio` installed to build and run projects that depend on it.


## Task 2: Using Large Language Models to take in the transcription input and generate answers.

I am going to test multiple large language models on various matrics the list of models is as follows:

1. LLAMA 3 [https://github.com/meta-llama/llama3]
2. LLAMA 2 [https://github.com/meta-llama/llama]
3. GPT 2 [https://github.com/openai/gpt-2/tree/master]
4. FALCON [https://huggingface.co/tiiuae/falcon-40b]
5. MISTRAL [https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.2]

### Dependencies required this dependencies may change over time as this models keep updating and may require some additional installations in the future:

torch

fairscale

fire

sentencepiece

regex

requests

tqdm

## Prerequisites

This part also requires the following tools:

- **wget**: Needed for downloading data.
- **md5sum**: Used to verify the integrity of downloaded files.

### Installation

#### Linux
- Debian/Ubuntu: `sudo apt-get install wget coreutils`
- Red Hat/Fedora: `sudo dnf install wget coreutils`

#### macOS
- Install Homebrew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- `brew install wget`
- `brew install coreutils` (provides `gmd5sum`)

#### Windows
- Install Chocolatey: Follow instructions at https://chocolatey.org/install
- `choco install wget`
- `choco install md5deep`

Please replace these commands with appropriate equivalents if you are using a different package manager or installation method.






