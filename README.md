  Telegram online status logger bot.

  Uses Telethon library to check online status and if it was changed send you a message.

  Because of telethon has a time limitation between requests.
  

Install

  pip install telethon
 
Setup

Create your telegramm application on https://my.telegram.org/apps and replace API_HASH, API_ID to yours.

API_HASH = 'your api hash'
API_ID = 'yuor api id'

Create bot in your telegram client (write a message to @BotFather) and copy bot token into app

bot = TelegramClient('bot', API_ID, API_HASH, connection=connection.ConnectionTcpMTProxyRandomizedIntermediate,
    proxy=proxy).start(bot_token='YOUR BOT TOKEN')

Run

  python spy.py
  
  Then input your telegram account number which will be sending requests to get users online status.
  
  Input  code in console from telegram.
  
  Done.
  
  Write /help to your bot to see usage information.
