# Ethos BotManagement - UI Structure and Layout

This EthosProject Module is used to keep track of, add, remove, and delete Telegram Bot Accounts.  Telegram Bot accounts will be used as our Agents that will go and perform many different tasks needed.  

Telegram bots are tied to verified Telegram accounts and any Telegram account may configure as many bots as they want.  These bots can then be deployed to enter into channels for monitoring or actions, or can monitor channels externally and outside of channels (IE:  Have not joined them).  

A single bot account can run many different tasks for any single channel depending on the code within the bot logic.  

## The UI Interface
### Display of existing Telegram Bots that are configured within the EthosProject Telegram Modules section.
- The UI layout should be similarly laid out like the Ethos-OCR module is - the top portion of the screen is the display of the selected bot which should show the notes and details about the selected bot record.
  - The bottom should be a visualizer of all of the bots accounts (similar to the OCR record visualizer)

### Adding New Bot Accounts
- We need the option to ADD new bots, via a button, to then provide information about the bot.  As it stands now, bots will be manually created on one of our verified Telegram accounts through interactions with @botfather on Telegram.
- When adding a new bot, the form should ask several questions.  In the future this will be much more dynamic and automated but for now, we'll just add in the information manually into the form after clicking ADD.


##### Add User Form Fields

When an admin click ```ADD``` to add in a new Telegram bot, there will be a dialog window that will gather the information below.

- Bot Username:  The Bot Username should be the same name that was used to name the bot.  Note, this is different than the actual @ bot name.  This Username can be anything and different from the Bot Name.
- Bot Name: This is the telegram name for the bot and it must end with bot, _bot, -bot.  This is a hard requirement for Telegram.
- Bot 

We can add more statistics for these configured bots later, but for now, we just need these to be in a database that can be access by the EthosProject.  Eventually, the ID of the bot will be used in other modules and databases but for now, let's just make this basic to get the foundation laid.

