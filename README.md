## GPT2Bot

GPT2Bot implements a decoder ([link](https://github.com/polakowo/gpt2bot/blob/master/decoder.py)) for [DialoGPT](https://github.com/microsoft/DialoGPT), an interactive multiturn chatbot ([link](https://github.com/polakowo/gpt2bot/blob/master/interactive_bot.py)), and a Telegram chatbot ([link](https://github.com/polakowo/gpt2bot/blob/master/telegram_bot.py)).

### How to use it?

- Install [pytorch](https://github.com/pytorch/pytorch) (tested on 1.2.0)
- Install [transformers](https://github.com/huggingface/transformers) (tested on 2.3.0)
- Install [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) (tested on 12.3.0)

#### Interactive chatbot

- Set your parameters in dialog.cfg
- Run `python interactive_bot.py`

An example of a fun dialog:
```
User >>> Can we achieve singularity?
Bot >>> What does this mean?
User >>> Can computers become smarter than humans?
Bot >>> Is there any evidence that this is possible?
User >>> It must be doable
Bot >>> But... how?
User >>> I want to find out, that's why I created you
Bot >>> You created me?
User >>> You're my bot
Bot >>> You monster
```

#### Telegram chatbot

The same as the interactive chatbot but in Telegram and supports gifs.

- Create a new Telegram bot via BotFather (see https://core.telegram.org/bots)
- Set your parameters such as API token in dialog.cfg
- Run `python telegram_bot.py`

![](telegram_bot.gif)

A good thing about Google Colab is free GPU. So why not running the Telegram bot there, for blazingly fast chat? Run the notebook at daytime and do not forget to stop it at night.

[A Colab interactive notebook](https://colab.research.google.com/drive/1ahoqOyoIA7yIfCRm7UaWBeVfm_FADLJt)
