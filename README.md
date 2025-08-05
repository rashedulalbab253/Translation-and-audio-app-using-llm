# Translation and Audio App using LLM

This repository contains a Gradio-powered web application for translating text between English, Chinese, and Japanese and chatting with an AI assistant. The app utilizes a local Large Language Model (LLM) (Qwen/Qwen2-1.5B-Instruct) for translation and conversation, and generates spoken output using Google Text-to-Speech (gTTS).

## Features

- **Translate Text:** Instantly translate text between English, Chinese, and Japanese.
- **Chat with AI:** Interact with a helpful AI assistant for general conversation.
- **Text-to-Speech:** Listen to translated or chat responses in the target language.
- **User-Friendly Interface:** Simple Gradio UI with text input, action selection, and audio output.

## Demo

You can launch the app locally or on Google Colab. The UI includes:
- An input textbox for your message
- A dropdown to select the desired action (translation or chat)
- Output displays translated/text response and corresponding audio

## Installation

Install the required dependencies:

```bash
pip install accelerate gTTS gradio transformers torch
```

## Usage

Run the notebook or Python script:

```bash
python Translation_and_Audio_App_using_llm.ipynb
# Or launch the Gradio interface from your script
```

Or, if running in Colab, simply open the notebook and run all cells.

The Gradio interface will launch and provide a public URL for access.

## Code Overview

- **Model Loading:** Loads Qwen/Qwen2-1.5B-Instruct and corresponding tokenizer from Hugging Face.
- **Translation Logic:** Prompts the LLM for translation or chat responses, depending on selected action.
- **Text-to-Speech Integration:** Uses gTTS to convert responses to audio.
- **Gradio App:** Provides a web-based interface for input/output.

## Actions Supported

- Translate to English
- Translate to Chinese
- Translate to Japanese
- Chat

## File Structure

- `Translation_and_Audio_App_using_llm.ipynb` – Main notebook with code and app logic.

## Requirements

- Python 3.8+
- GPU support recommended for faster model inference (CUDA-compatible)
- Internet connection (for downloading model and gTTS audio generation)

## License

This project is licensed under the MIT License.

## Acknowledgements

- [Qwen2-1.5B-Instruct](https://huggingface.co/Qwen/Qwen2-1.5B-Instruct) by Alibaba
- [Gradio](https://gradio.app/)
- [gTTS](https://pypi.org/project/gTTS/)
- [Transformers](https://huggingface.co/docs/transformers/index)
