# Multilingual Translator

A Streamlit-based multilingual translator using HuggingFace **MarianMT** models for neural machine translation, with automatic language detection.

## Features

- 🌍 Supports multiple language pairs via Helsinki-NLP MarianMT models
- 🔍 Automatic source language detection using `langdetect`
- ⚡ Real-time translation via Streamlit UI
- 🚀 Deployable on Google Colab with ngrok

## Tech Stack

- [`transformers`](https://huggingface.co/docs/transformers) — MarianMTModel & MarianTokenizer
- [`langdetect`](https://pypi.org/project/langdetect/) — Language detection
- [`streamlit`](https://streamlit.io/) — Frontend UI
- [`pyngrok`](https://pyngrok.readthedocs.io/) — Colab tunnel deployment

## How to Run

### Option 1: Google Colab
1. Open `Multilingual_Translator.ipynb` in [Google Colab](https://colab.research.google.com/)
2. Run all cells
3. Authenticate ngrok when prompted
4. Access the public Streamlit app link

### Option 2: Local Setup
```bash
git clone https://github.com/Kunal04041/Multilingual-translator.git
cd Multilingual-translator
pip install -r requirements.txt
streamlit run app/main.py
```

## Project Structure

```
Multilingual-translator/
├── app/
│   ├── main.py              # Streamlit entry point
│   ├── translator.py        # MarianMT model logic
└────config.py            # Language pair configs
├── notebooks/
│   └── Multilingual_Translator.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## Supported Language Pairs

| Source | Target |
|--------|--------|
| English | French |
| English | German |
| English | Spanish |
| English | Hindi |
| French | English |

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.
