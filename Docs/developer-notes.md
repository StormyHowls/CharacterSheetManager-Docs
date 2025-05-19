# Dev Notes

## Technologies Used
- C# (.NET 9)
- DSharpPlus for Discord bot framework
- ClosedXML for Excel generation
- Entity Framework Core (EF Core) for SQL handling
- Docker for deployment and portability

## Known Limitations
- Character creation resets if the user disconnects or the bot restarts (no persistent session handling yet)
- Discord file delivery limited by file size cap (typically 8MB for standard users)
- No real-time combat management (currently sheet export and static tracking only)

## Future Features
- Experience to spendable point exchange
- Merits and Flaws system
- Gift acquisition and tracking
- Ability Specialties
- Pack and Sept affiliation tracking
- Replace manual GUID entry with Discord buttons for smoother user interaction
- Character roles within their pack and factions
- Totem assignment and tracking
- Full point transaction audit log

## Wish List
- API integration to upload character sheets to Roll20.net
- Auto-battler or real-time combat module within Discord
- Unity integration for future visual expansions

### Notes:
This project is designed to be modular and expandable. Features are prioritized based on player usability, storyteller functionality, and long-term maintainability.