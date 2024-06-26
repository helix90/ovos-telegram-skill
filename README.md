# <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/paper-plane.svg' card_color='#0088CC' width='50' height='50' style='vertical-align:bottom'/> Telegram
A skill to control your Mycroft instance through a TelegramBot.

## About 

You need to create a telegram bot (via BotFather) and save the Bot Token, your ChatID and your MyCroft Device name on home.mycroft.ai under skill settings.
You can now commmunicate with your MyCroft Unit via this bot.

Settings:
- BOT TOKEN (MANDATORY): Your bot token you got from BotFather
- DEVICE NAME (CASE SENSITIVE | MANDATORY): Your Device name you configured on home.mycroft.ai - Devices - Registered Devices
- BOT TOKEN SECOND MYCROFT DEVICE (OPTIONAL): If you have a second Mycroft Device and you want to use this skill with it -> put your second bot token here (it has to be an other bot than the first one because telegram only allows one device to get updates from one bot)
- SECOND MYCROFT DEVICE NAME (IF YOU HAVE A SECOND DEVICE): Your Device name from your second Device you configured on home.mycroft.ai - Devices - Registered Devices
- PRIMARY USERNAME (OPTIONAL): You do not need to put anything here, the skill does not use this field. It is only for yourself to know which Chat ID belongs to whom
- PRIMARY CHAT ID (MANDATORY): You will get your Chat ID from the Telegram-Skill if you have configured BOT TOKEN (first field) and DEVICE NAME, saved and then write anything to the bot.
- SECOND USERNAME (OPTIONAL): For second User if you have one
- SECOND CHAT ID (IF YOU HAVE A SECOND USER): Same as PRIMARY CHAT ID with Telegram-Account of second user

Detailed HowTo:

- Install this skill on your Mycroft Device

- Create a telegram bot:
Open Telegram App on your smartphone, click on the search symbol in the upper right corner<br/>
Search for BotFather and click on it<br/>
Now type /newbot hit enter<br/>
Botfather should reply with: Alright, a new bot. How are we going to call it? please chosse a name for your bot.<br/>
Give your bot a displayname like Mycroft<br/>
Botfather should reply with: Good. Now let's choose a username for your bot. It must end in bot. Like this, for example: TetrisBot or tetris-bot.<br/>
Give your bot unique username like lukesmycroftbot<br/>
Botfather should now give you your token for this bot<br/>
Save this token and don't post it online or send it to people, safety first!<br/>

Telegram documentation on botfather: https://core.telegram.org/bots#6-botfather

- Edit the settingsmeta.yaml file in the telegram-skill folder on your Mycroft Device

- Copy/paste your token botfather gave you in the field TeleToken1 (MANDATORY)

- Copy/paste your device name into MDevice1 (CASE SENSITIVE | MANDATORY)

- SAVE and confirm that the settings are synced to your Mycroft Unit

- Open Telegram App on your smartphone and search (upper right corner) for your bot (username or displayname) click on it and write test or hello to your bot
  It should respond with: This is your ChatID: YOURCHATID

- Copy/paste this into settingsmeta.yaml as User1 (MANDATORY)

- SAVE and confirm the settings are synced to your Mycroft Unit

- On every reboot your bot should send you this welcome message: Telegram-Skill on Mycroft Unit YOURUNIT is loaded and ready to use

## Credits 
Forked from - Lukas Gangel (@luke5sky)
Updated by - Robert A (@helix90)


## Category
IoT
**Productivity**

## Tags
#messenger
#bot
#telegram-bot
