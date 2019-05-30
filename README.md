![Build status](https://img.shields.io/travis/hellodhlyn/telegrambot-py.svg?style=flat-square) ![Coverage](https://img.shields.io/codecov/c/gh/hellodhlyn/telegrambot-py.svg?style=flat-square) ![License](https://img.shields.io/github/license/hellodhlyn/telegrambot-py.svg?style=flat-square)

# telegrambot-py

> Make your own telegram bot easily.

## Getting Started

Before starting, you need to create a bot and get a token for it. For details, see instructions [here](https://core.telegram.org/bots#3-how-do-i-create-a-bot).

Below is the example code that responds 'pong' for '/ping' command.

```python
from telegrambot import Bot

bot = Bot('your_bot_token')

@bot.command('/ping')
def ping(ctx):
    return 'pong'

bot.start()
```

## Development
### Prerequsites

- Python 3.4 or greater
- [Pipenv](https://github.com/pypa/pipenv)

### Install dependencies

```sh
pipenv install --dev
```

### Running Tests

```sh
pipenv run lint
pipenv run test
```
