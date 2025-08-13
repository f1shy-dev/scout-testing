# scout-testing

A comprehensive testing repository containing themed test data and file editing demonstrations for various development scenarios.

## Repository Contents

### 📁 Root Files
- `README.md` - This documentation file
- `THEME_TEST_FILES.md` - Detailed documentation about the themed test files and their usage scenarios

### 🧪 File Editing Demo (`file-editing-demo/`)
*Persona RPG-themed demonstration of advanced file editing capabilities*

- `README.md` - Complete documentation of editing capabilities and performance metrics
- `initial_data.json` - Complex nested JSON with persona data, social links, battle records, and exploration stats (167 lines)
- `game_config.yaml` - Hierarchical YAML configuration with game settings, calendar system, and performance options (79 lines)
- `skills_database.csv` - Tabular CSV data with skill information, ranks, and special effects (16 entries)

### 📱 Neko Atsume Theme (`neko-atsume/`)
*Japanese mobile cat collecting game data for comprehensive testing scenarios*

- `cats.json` - Complete cat database with regular and rare cats (5 regular + 3 rare cats)
- `food_data.json` - Food types, costs, and feeding strategies
- `game_config.yaml` - Game configuration and mechanics settings
- `player_progress.txt` - Realistic player progress log spanning 42 days
- `test_scenarios.md` - 36 comprehensive test scenarios covering functionality, edge cases, performance, and UI/UX
- `toys.csv` - Toy/goodies data with costs and attractiveness ratings (11 different toys)

### 🏝️ Summer Pockets Theme (`summer-pockets/`)
*Visual novel game data from Key's emotional island-based story*

- `characters.json` - Complete character database with all heroines (8 total: 4 original + 4 Reflection Blue)
- `dialogue_samples.txt` - Authentic dialogue samples from various story routes
- `island_locations.csv` - All game locations with accessibility and atmosphere data (15 locations)
- `music_tracks.json` - Comprehensive soundtrack information (47 tracks with emotional categorization)
- `routes_config.yaml` - Story route structure and unlock conditions (10 routes, 52+ hour total playtime)
- `test_scenarios.md` - 60 detailed test scenarios covering story routes, technical functionality, and content validation

## File Format Coverage

### Data Formats
- **JSON Files**: 6 files (structured data for characters, cats, food, music, personas)
- **YAML Files**: 3 files (configuration files for game settings and routes)
- **CSV Files**: 3 files (tabular data for toys, locations, skills)
- **TXT Files**: 2 files (progress logs and dialogue samples)
- **Markdown Files**: 4 files (test scenarios and documentation)

### Total Statistics
- **18 data files** across 4 directories
- **4 documentation files**
- **Multiple complexity levels**: Simple key-value pairs to complex nested hierarchies
- **96 test scenarios** total (36 Neko Atsume + 60 Summer Pockets)
- **Mixed data types**: Strings, numbers, booleans, arrays, nested objects
- **Real-world themed content** beyond generic test data

## Usage Scenarios

These themed test files are designed for:

- **File Processing Tests**: Parsing different formats (JSON, CSV, YAML)
- **Data Validation**: Schema validation and data integrity checks
- **Performance Testing**: Loading and processing various file sizes
- **Content Management**: Testing search, filter, and organization features
- **Localization Testing**: Character encoding and multilingual content
- **API Testing**: Using as mock data for endpoints
- **Database Testing**: Import/export functionality validation
- **File Editing Demonstrations**: Complex multi-format editing scenarios

All themes provide rich, realistic data that makes testing more engaging and closer to real-world scenarios than generic Lorem ipsum content.
