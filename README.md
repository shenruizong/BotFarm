Console application to spawn WoW automated players.

Credit for the authentication process and the base implementation goes to mangos, WCell, PseuWoW and TrinityCore.

The application configuration is setup by editing the *.config file in the output folder:
- fill the [Username](BotFarm/App.config#L17) and [Password](BotFarm/App.config#L20) fields with an account with ".account create" permissions to allow the BotFarm to automatically create new accounts when required. Make sure this account has already a character.
- fill the [Min](BotFarm/App.config#L35)/[MaxBotsCount](BotFarm/App.config#L32) with the amount of bots you want to connect at same time. This will automatically create new accounts when required
- set paths for [MAPsFolderPath](BotFarm/App.config#L53), [VMAPsFolderPath](BotFarm/App.config#L50) and [MMAPsFolderPath](BotFarm/App.config#L47)
- make sure to read [README.md in BotFarm/lib folder](BotFarm/lib/README.md) too with additional steps about required dependencies

Write "stats" in the console to view some statistics about the current status of bots.
Write "quit" to cleanly shut down the application and persist the new connection infos to botsinfos.xml file.