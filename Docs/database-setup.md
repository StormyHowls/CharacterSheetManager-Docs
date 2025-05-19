# Database Setup

## Requirements

- SQL Server (local or Docker) ~ This project was done with Docker.
- SSMS (SQL Server Management Studio) or Azure Data Studio
- The DatabaseSeed.sql file included with this project

## Instructions

1. Create a New Empty Database
   -  Name it CharacterSheetDB
   -  Use default settings unless otherwise needed.
2. Run the Database Seed Script
   - Open DatabaseSeed.sql in SSMS or your SQL tool of choice.
   - Connect to your SQL Server instance.
   - Ensure your context is switched to the CharacterSheetDB database.
   - Execute the script.
   - This will create all necessary tables and insert starting data.
3. Update the Bot's config.json (if needed)
   - Ensure your connection string points to the correct server and database.
   - Example config.json entry:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost,1433;Database=CharacterSheetDB;User Id=sa;Password=your_password;"
  }
}
```

### Notes
- The database is pre-populated with:
  - Species, Tribes, Breeds, Auspices
  - Attributes, Abilities
  - Backgrounds and Restrictions
  - Resources and Renown types
- No migrations are necessary; the seed file handles both schema and data.