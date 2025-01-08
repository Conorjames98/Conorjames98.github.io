+++
date = '2025-01-04T01:57:11Z'
draft = false
title = 'A discord bot'
pin = false
+++

# Discord bot

I began working on a small discord bot to understand how it works in python, like many things in python to make life easier we have things like libaries in this case it is the discord.py libary which allows us to interact with discord in ways that aren't as complex as they would be without it. these shothands such as "@bot.command" are called a decorator.

Some things I learnt along the way

1) Never hardcode your discord token into your bot's code.

What I did was store this token in a .env file which requires the python-dotenv libary to load the token into the bots enviroment, as I used github to upload my repos of course I also did not want to upload this .env file to github or my token would be exposed to the internet (fun fact if you accidently end up doing this like I did discord will tell you the exact location of the token on the internet and it will also force change your current token)

2) the discord.py libary contains numerous decorators to make life easier when wanting to do specific things like commands or bot events.