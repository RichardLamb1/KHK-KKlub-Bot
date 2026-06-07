# Installation
Create a file (if it doesn't already exist) called `config.json` with the following:
```
{

"check_kklub_leaderboard" : "Show kklubs of every user",
"add_kklub" : "REPORT A KKLUB VIOLATION",
"remove_kklub":"remove kklub for a user <ADMINISTRATOR>" ,
"check_kklubs":"checks how many kklubs you have (hopefully it's zero)" ,
"reset_kklubs":"resets KKlub Database <ADMINISTRATOR>" ,
"help" : "Show all command and description",
"check_pin_report_leaderboard" : "Show pin reports of every Pledge",
"add_pin_report" : "REPORT A PIN VIOLATION",
"remove_pin_report":"remove pin report for a Pledge <ADMINISTRATOR>" ,
"check_pin_report":"checks how many pin reports you have (hopefully it's zero)" ,
"reset_pin_reports":"resets Pin Report Database <ADMINISTRATOR>" ,
"add_blacklist": "Add a person making false kklub reports  <ADMINISTRATOR>",
"remove_blacklist": "Remove person from the WALL OF SHAME  <ADMINISTRATOR>",
"check_blacklist": "To see if you're on the WALL OF SHAME (hopefully not)",
"wall_of_shame": "The wall of shame",
"reset_blacklist": "reset the WALL OF SHAME database <ADMINISTRATOR>",
"bot_token" : ""

}
```
Go to [Discord's developer portal](https://discord.com/developers/home) and create a new application. Select `bot` from the left sidebar and generate a token. Paste the bot_token from Discord in the config.json file.

Still under the `bot` category of Discord's developer portal, scroll down to `Privileged Gateway Intents` and enable all three switches.

Run `python3 -m venv venv` then `source venv/bin/activate` to create a Python virtual environment. Then run `pip install discord` to install the dependency.

Finally, run `python3 bot.py` to start the bot!

# Commands
## Basics
There are five available commands that this bot can understand:
```
  /add_kklub <username>
  /remove_kklub <username>  //Needs Administrator Privileges
  /check_kklub
  /check_leaderboard
  /reset //Needs Administrator Privileges
```
Adds a kklub to a user
```
  /add_kklub <username>
```
Removes a kklub for a user
```
  /remove_kklub <username>  //Needs Administrator Privileges
```
Returns number of kklubs for invoker of command
```
  /check_kklub
```
  
Will show all players using an embedded table and reaction page changer

```
  /check_leaderboard
```
The following command will reset the database:
```
  /reset //Needs Adminstrator Privilages
```
