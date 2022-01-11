# TIME WMEMO Large Order Tracker

A telegram bot that notifies when there are orders greater than $100,000 for TIME/MIM on Traderjoe and wMEMO/MIM on SushiSwap.

## Table of Contents

1. [About the Project](#about-the-project)
2. [Getting Started](#getting-started)
3. [Dependencies](#dependencies)
4. [TODO](#todo)

## About the Project
The bot uses decentralized exchange (DEX) transactions data from dexscreener.com and notifies when there are unusually large orders. The threshold for large orders can be set manually. You can also add your own pairs manually in the code.

More improvements will be added in the future such as custom support for commands for user customisation directly on Telegram.

## Getting Started

1. Download or clone the project:

```
$ git clone https://github.com/wdwdwdwdwdwdwd/TIME-WMEMO-Large-Order-Tracker.git && cd TIME-WMEMO-Large-Order-Tracker.git
```

2. Create a Telegram bot using BotFather on Telegram. [Here is how you do it.](https://sendpulse.com/knowledge-base/chatbot/create-telegram-chatbot)

3. Create a file `.env` in the same folder as the bot and add
```
API_KEY = '<YOUR API KEY HERE>'
```

4. Create a channel on Telegram and use [ID Bot](https://t.me/username_to_id_bot) to find out your channel ID.

5. Add the channel ID on a new line in your `.env` file.
```
CHAT_ID = '<YOUR CHAT ID HERE>'
```

6. Run the script and check for missing dependencies and install them
```
$ python3 bot.py
```

7. Run the bot again and now it should show you almost in real time when there are unusually large orders for the trading pairs you've inputted.
```
$ python3 bot.py
```

## Dependencies

- Python 3
- python-dotenv

## TODO

- [ ] Try to get actual data using a DEX API instead of borrowing from Dexscreener
- [ ] Save local logs of large orders using CSV
- [ ] Make the bot customisable using Telegram
- [ ] Maybe copy trades automatically from certain wallets in the future(?)
