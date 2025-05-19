# Character Sheet Manager

A character sheet manager for the tabletop role-playing game Werewolf: The Apocalypse.

Although heavily inspired by the game, this is not an official product of White Wolf Publishing, Inc. or any of its affiliates. The game is a work of fiction; any resemblance to actual persons, living or dead, is purely coincidental.
[Click here for Video Presentation](https://www.youtube.com/watch?v=PDU1XRehry0&t=795s)

## Features

- **Discord Bot:** Manage characters and campaigns directly within Discord.
- **User Registration:** Utilizes Discord usernames to register users in the database.
- **Chronicle Management:** Storytellers can create and manage multiple chronicles.
- **Character Creation:** Wizard-like interface for creating and managing characters.
- **Dynamic Features:** Availability of features based on user roles and character aspects.
- **Character Profiles:** View and edit character sheets with all necessary information.
- **Tracking:** Monitor character stats, abilities, renown, resources, and points.
- **Excel Export:** Export character data into a formatted Excel document styled for Werewolf.

## Getting Started

- Invite the bot to your server or join our Discord.
- Use !help to view available commands.
- Register your username with !register.
- Join or create a chronicle using !joinchronicle or !createchronicle.
- Create your first character with !createcharacter.
- Update attributes and abilities using !updateattributes.
- Allocate background points with !updatebackgrounds.
- Export your character sheet with !exportcharacter.

## Technologies Used

- C# (.NET 9)
- DSharpPlus for Discord integration
- ClosedXML for Excel generation
- Entity Framework Core (EF Core) for SQL handling
- Docker for deployment

## Known Limitations

- Character creation resets if the user disconnects or the bot restarts (no persistent session handling yet).
- Discord file delivery is limited by Discord's file size cap (typically 8MB for standard users).
- No real-time combat management; currently supports sheet export and static tracking only.

## Future Features

- Experience to spendable point exchange system.
- Integration of Merits and Flaws.
- Gift acquisition and tracking.
- Ability Specialties.
- Pack and Sept affiliation tracking.
- Replace manual GUID entry with Discord buttons for smoother user experience.
- Character role assignment within packs and factions.
- Totem assignment and tracking.
- Full point transaction audit log.

## Wish List

- API integration to upload character sheets to Roll20.net.
- Auto-battler or real-time combat module within Discord.
- Unity integration for future visual expansions.

## Documentation

For detailed information, refer to the following documents:
- [Index](Docs/index.md)
- [Excel Export](Docs/excel-export.md)
- [Discord Commands](Docs/discord-commands.md)
- [Data Sources](Docs/data-sources.md)
- [Database Setup](Docs/database-setup.md)
- [Terms of Service](Docs/TOS.md)
- [Privacy Policy](Docs/PRIVPOL.md)

## Configuration

This project uses `.env` and `config.json` files to manage secrets and settings.

### Setup

- Copy `.env.example` to `.env` and fill in your values
- Copy `config.example.json` to `config.json` and update it

**Never commit real credentials to Git.**

## License

This project is licensed under the [MIT License](LICENSE.txt).
