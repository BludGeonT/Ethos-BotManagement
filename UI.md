# Ethos BotManagement - UI Structure and Layout

This EthosProject Module is used to keep track of, add, remove, and delete Telegram Bot Accounts.  Telegram Bot accounts will be used as our Agents that will go and perform many different tasks needed.  

Telegram bots are tied to verified Telegram accounts and any Telegram account may configure as many bots as they want.  These bots can then be deployed to enter into channels for monitoring or actions, or can monitor channels externally and outside of channels (IE:  Have not joined them).  

A single bot account can run many different tasks for any single channel depending on the code within the bot logic.  

## The UI Interface
### Display of existing Telegram Bots that are configured within the EthosProject Telegram Modules section.
- There should be a place on the screen that formats nicely and displays the currently configured bots that are ready to go in the system.  Eventually we will have TAGS that are assigned to them, etc but for now, the list of added Telegram Bots and their information should be displayed on the screen.  Within this pane, as each bot is shown, there should be a way to EDIT the bots' information, a button to DELETE bots, and a button to DISABLE or ENABLE the bots and the ability to select one or more for these actions should exist.

### Adding New Bot Accounts
- We need the option to ADD new bots, via a button, to then provide information about the bot.  As it stands now, bots will be manually created on one of our verified Telegram accounts through interactions with @botfather on Telegram.
- When adding a new bot, the form should ask several questions.  In the future this will be much more dynamic and automated but for now, we'll just add in the information manually into the form after clicking ADD.


### Add User Form Fields

When an admin click ADD to add in a new Telegram bot, there will be a dialog window that will gather the information below.

- Bot Username:  The Bot Username should be the same name that was used to name the bot.  Note, this is different than the actual @ bot name.
- Bot Name: This is the telegram name for the bot and it must end with bot, _bot, -bot.  This is a hard requirement for Telegram.
- Telegram Account:  This will be the ID of the Telegram account that created the bots in @botfather channel
- Role:  This should be a dropdown choice and it will contain the roles that the bot uses.  For now, we can add the 6 MODULES that we have configured in the Telegram section as these choices

We can add more statistics for these configured bots later, but for now, we just need these to be in a database that can be access by the EthosProject.  Eventually, the ID of the bot will be used in other modules and databases but for now, let's just make this basic to get the foundation laid.

