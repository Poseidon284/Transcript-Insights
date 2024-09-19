# Audio/Video Transcription, Topic Recognition, and Summarization

## Overview
This project processes audio and video files to generate transcripts, recognizes topics using the **Latent Dirichlet Allocation (LDA)** model, and provides summarization using a **Large Language Model (LLM)** with **Retrieval-Augmented Generation (RAG)**.

### Key Features:
1. **Audio/Video Input**: Accepts multiple formats of audio and video files.
2. **Transcription**: Automatically converts speech from the input files into text using speech-to-text technology.
3. **Topic Recognition**: Identifies main topics from the transcript using the LDA model.
4. **Summarization**: Produces concise summaries of the transcripts using RAG, which improves accuracy by pulling relevant information from a database during the generation process.

## Architecture
1. **Input Stage**: Audio/Video files are uploaded to the platform.
2. **Transcription Stage**: Files are processed by a speech-to-text engine (using **Whisper**).
3. **Topic Recognition Stage**: LDA model extracts major topics from the transcript.
4. **Summarization Stage**: LLM RAG model generates concise summaries, retrieving relevant data from a knowledge base as needed.
5. **Output**: The project can return a transcription to the audio or video file, recognize topics using LDA, and summarize the transcript.

### Workflow
- **Audio/Video Input → Speech-to-Text → Transcript**
- **Transcript → Topic Recognition (LDA)**
- **Transcript + Topics → Summarization (LLM RAG)**

### Files and Directories
- `c5ids.ipynb`: Handles the speech-to-text conversion, Performs topic modeling using LDA, Summarizes the transcript using the RAG approach.

## Dependencies
- **Speech-to-Text**: `whisper`
- **LDA Topic Modeling**: `gensim`
- **Summarization (RAG)**: `langchain`, `gemini_ai` 

## Future Improvements
- Implement integration of actions and create a linear flow in the project.
- Add "QnA" along with transcription and summarization.
- Improve topic modeling by tuning the LDA model.
- Enable more granular control over the summarization (length, style, etc.).


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Contact
For inquiries or support, please email `radheshrathnam28@gmail.com`.

## Author
Radhesh Rathnam
