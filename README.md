# Gpt-4

A small Gradio chat UI wrapping the OpenAI ChatCompletion API (`gpt-3.5-turbo`) — a learning exercise with the OpenAI API, not an OpenAI project.

## How it works
`app.py` keeps a running conversation (system + user + assistant messages) and sends it to `gpt-3.5-turbo` on each turn, displaying the reply in a simple Gradio textbox interface.

## Running locally
```bash
pip install openai gradio
export OPENAI_API_KEY=your_key_here   # Windows: set OPENAI_API_KEY=your_key_here
python app.py
```
The API key is read from the `OPENAI_API_KEY` environment variable — never hardcoded.
