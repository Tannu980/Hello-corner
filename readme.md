# Hello Corner 👋

> A calm place to practice talking. No audience, no judging, no rush.

I built this for a friend in my college. She is quiet, and talking to new people is hard
for her. Her goals are to make a good friend circle, find ideas for a startup, and lose
her stage fear. I can't do that for her, but I could give her a safe place to practice.

The AI runs **on your own computer** (through [Ollama](https://ollama.com)), so nothing
you type is sent to the internet.

## What you can do here
- **Chat with a friend:** easy small talk with "Sam", one gentle question at a time.
- **Startup ideas:** a friendly mentor helps you find ideas from everyday college problems.
- **Practice a talk:** say a short intro and get one thing you did well, one small tip, and one audience question.

There is also a mic button (speak instead of typing), a "practice days" counter, and a tiny
daily challenge, like "say hi to one classmate". Practice here is meant to lead to real
conversations, not replace them.

## How to run it
1. Install [Ollama](https://ollama.com), then in a terminal run: `ollama pull llama3.2:3b`
2. Start the website: `python server.py`
3. Open http://localhost:8000 (use Chrome or Edge if you want the mic button)

Want a different model? `HELLO_MODEL=qwen2.5:3b python server.py`

## What is in each file
| File | What it does |
|------|--------------|
| `server.py` | Shows the website and passes your messages to the AI. The 3 personalities live here. |
| `static/index.html` | The page layout. |
| `static/style.css` | The warm colours and spacing. |
| `static/app.js` | The chat, the mic button and the practice-day counter. |

There are no frameworks and nothing to `pip install`, so it should be easy to read and change.
To change how Sam talks, edit the `PERSONAS` text in `server.py`. It is just plain English.

## Ideas for you to add
- An interview practice mode
- Hindi or other languages
- A softer voice that reads the replies out loud

## License
MIT. Fork it, change it, build one for your own friend. 💛
