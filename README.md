# VerifyBot   

**Note: This software is no longer maintained. Please do not message me asking for help**

[![Build Status](https://travis-ci.org/seasniffer/VerifyBot.svg?branch=master)](https://travis-ci.org/seasniffer/VerifyBot)   

A bot that uses the Discord.NET and Guild Wars 2 API's to verify what world a users account is on. Made for Jade Quarry Discord but open source for all to use.   

You'll need a verified rank in Discord and a #verify text channel. When a user types !verify the bot will message them with instructions. Once a user is verified an entry is made into a SQLite database and the user is given the verified rank.

You'll need to add a secrets.json file to the directory that the executable is running from. Here are the required fields.
```
{
	"WorldIds": [ 1008, 1001, 1013 ],
	"ServerId": your_discord_server_id_here,
	"DiscordToken": "your_discord_bot_token_here",
	"VerifyRole": "your_verified_role_name_here"
}
```
