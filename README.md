# Ethos-BotManagement

#### Summary
This module is to manage the Telegram Bot Accounts that we create from a verified Telegram account.  These bots will be all stored together and act as a pool of bot agents that can then be assigned to Telegram channels through other EthosProject Modules.  Other EthosProject modules will be able to grab one of these bots to use for their Module's workflow.  

#### Module Highlights
- This module will be used to register bot accounts created by @botfather on Telegram.  A normal, registered Telegram account can create an unlimited amount of bots using @botfather and each of these accounts will generate an API Key.
- This module will be initially used to record the bots that have been created by @botfather on Telegram and this information will be input into the UI and their information will be stored in a secure Database.

##### Database Information
  - Item that will be stored in the secure database but other trusted modules will need to be able to view the information within these database records.
    - The Bot Name (This can be anything) let's say up to a max of 50 characters in the database
      - For now, this will be manually created and manually entered into the Bot creation tool in Ethos-BotManagement
      - Database field name:  ```BOT_NAME```
    - The Bot Username (This can be anything but MUST end with bot).  This will be the @ name for the bot.
      - For now, this will be manually created and manually entered into the Bot creation tool in Ethos-BotManagement
      - Database field name:  ```BOT_USERNAME```
    - The Bot API Key - This is a long string of text characters.  It is delimited by a colon (:) which separates the UID of the bot from the API Key.  Both of them together must be stored into this database field and record.
      - For now, this will be manually created and manually entered into the Bot creation tool in Ethos-BotManagement
        - Example of a full Bot API Key:  ```7551577597:AAGdliJXl4fxWNlOjNjAwzFUEb3162BBf0k```
          - UID section of the Bot:  ```7551577597```
          - API Key section of the Bot: ```AAGdliJXl4fxWNlOjNjAwzFUEb3162BBf0k```
      - Database field name:  ```BOT_APIKEY```
    - The Bot Notes - We want to have a field that can contain notes about the bot.  These notes can be added or edited within the Ethos-BotManagement module, but eventually will also be able to accept new notes from other modules that are utilizing one of these bots.  While adding a bot in the Ethos-BotManagement UI, the operator should be able to add in intial notes about the Bot and include a date and time stamp along with the name of the logged in operator.
      - After a bot has been saved into the Ethos-BotManagement table, then a button that says "ADD NOTES" can be pressed while a Bot is selected and the operator can add in a new set of notes and upon saving that, the same date and timestamp will be saved along with the Operator name.
        - This will allow for a bot to contain historical information or updates which might have valuable information such as during an investigation or prolonged operation to infiltrate, etc.
      - Database Field Name:  ```BOT_NOTES```
        - This field, over time, could accumulate lots of historical notes.  Almost like records within a field and perhaps a sort of JSON structure will work best here unless you have a better suggestion.
       
### User Interface (UI) Details

#### Refer to the UI.md file for the layout instructions and retaining all of the rules within the original PLANNING.md file.

- The Ethos-BotManagement Module UI will open up once Ethos-BotManagement is clicked from the left navigation panel from the EthosProject main page.
- The Ethos-BotManagement visual layout will be very similar to the Ethos-OCR module.



        

 

