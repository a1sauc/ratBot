## Purpose

This discord bot allows usesrs to record team kill statistics for a game. However, it is generic and can be configured to any game needed by editing database fields. 

## Bot Configuration

ratBot's commands are invoked by using the command prefix which is an exclamation mark. (!)

ratBot uses a database to record data in tables and is currently configured for MySQL 8.0.

1. Create a database connecction with bot
2. [Join the bot to your discord server]( https://discord.com/api/oauth2/authorize?client_id=986455489070108752&permissions=8&scope=bot )  

At this point you are ready to go, use !help command to learn more about ratBot's commands.

## Running in Development

The master branch is the latest working copy of the project. It should be considered unstable. 

## First Time Setup

`virtualenv venv && source env/bin/activate && pip install -r requirements.txt`

Runs on python version: 3.8.10

## Returning to an existing project

Be sure to activate the virtalenv

```
source venv/bin/activate
python src/ratBot.py
```

## Production Notes

* This was my first discord bot project and I used this guide to start. (https://realpython.com/how-to-make-a-discord-bot-python/)
* Note that when creating a bot, you may need to enable "Server Member intent" flag on the bot page in the Discord developers portal. 
* Delete function that deletes tables will be commented out initially. Later releases may have an edited version to only allow the "bot owner" to use the !delete command. 

## From Author

I am a undergraduate student at the University of Texas at Dallas. I wanted to make a discord bot to help my friends but also learn python and databases. I chose MySQL because of the online resources that are great for beginners. Thanks for checking out my work. 