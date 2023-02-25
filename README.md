# tmebot

Easy to write telegram bots framework with a system of routers.

Documentation:

+ [English](docs/index.md)

## Quick start

```shell
pip install tmebot
```

```python
import asyncio

from tmebot import Bot, TApp, types, start_polling

app = TApp()
bot = Bot("1:TOKEN")


@app.message()
async def message_handler(message: types.Message) -> None:
    await message.answer("Hello!")


if __name__ == "__main__":
    asyncio.run(start_polling(app, bot))
```

## Contact

[Telegram](toymac.t.me)
