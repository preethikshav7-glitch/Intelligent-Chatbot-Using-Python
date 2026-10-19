# Intelligent Chatbot using Python

An intelligent chatbot built with Python and basic Natural Language Processing (NLP). It understands user messages, identifies intent, and replies in real time. It uses only the Python standard library, so there is nothing to install.

## Features
- Intent recognition using text preprocessing and similarity scoring
- Typo correction (e.g. "pyton" is understood as "python")
- Remembers the user's name
- Tells the current time and date
- Safe calculator (e.g. `calculate 12 * 5`)
- Jokes, greetings, FAQs, and small talk
- Easy to extend: add new intents in the `INTENTS` list

## Requirements
- Python 3.9 or newer

## How to Run
```
python chatbot.py
```

## Example
```
You: hello
PyBot: Hi there! What can I do for you?
You: my name is Ravi
PyBot: Nice to meet you, Ravi!
You: calculate 12 * 5
PyBot: The answer is 60
You: bye
PyBot: Bye! Talk to you soon.
```

## Add Your Own Intent
```python
{
    "tag": "hours",
    "patterns": ["what are your working hours", "when are you open"],
    "responses": ["We are open 9 AM to 6 PM, Monday to Saturday."],
}
```

## Future Scope
- Machine learning intent classifier (scikit-learn)
- Web or Telegram bot interface
- Voice input and output
- Integration with OpenAI/Anthropic APIs for smarter replies
