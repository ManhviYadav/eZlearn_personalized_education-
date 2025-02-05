# EZLearn

## Overview
EZLearn is an automated system that facilitates educational content extraction and interactive learning from YouTube videos. The system downloads videos, converts them into audio, transcribes the content into text, generates questions, and provides an interactive multiple-choice quiz for users.

## Features
- **YouTube Video Extraction**: Fetches YouTube videos based on a search query, filtering by duration and language.
- **Video Downloading**: Downloads complete videos or extracts specific segments.
- **Audio Conversion**: Extracts audio from video files.
- **Speech-to-Text Transcription**: Uses OpenAI's Whisper model to transcribe audio into text.
- **Question Generation**: Generates questions from the transcribed text using an NLP model.
- **Interactive MCQ Quiz**: Presents users with multiple-choice questions to test their understanding.
- **SHA-256 Hashing**: Provides a function to generate a SHA-256 hash of given data.

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- `pip` package manager
- The required Python libraries:

```bash
pip install -r requirements.txt
```

### Additional Requirements
- `ffmpeg`: Required for video and audio processing. Install it using:

```bash
sudo apt install ffmpeg  # On Linux
brew install ffmpeg      # On macOS
winget install ffmpeg    # On Windows
```

## Usage
### Running EZLearn
To start the program, run:

```bash
python EZLearn.py
```

### Workflow
1. Enter a search query to fetch YouTube videos.
2. Select a video from the results.
3. Choose whether to download the entire video or specify a duration.
4. The system extracts audio, transcribes text, and generates MCQs.
5. Users can interact with the generated quiz and get their scores.

## File Structure after running the file
```plaintext
EZLearn/
├── EZLearn.py            # Main script
├── Audios/               # Stores extracted audio files
├── Transcribed_Text/     # Stores transcriptions
├── README.md             # Documentation
```

## License
This project is released under the MIT License.

## Author
Developed by Manhvi Yadav.
