# Theme Test Files

This repository contains test files organized around two popular gaming themes for comprehensive testing scenarios.

## 📱 Neko Atsume Theme

**About**: Neko Atsume is a beloved Japanese mobile game where players collect cats by placing toys and snacks in their yard. The game features over 40 different cats, including rare ones that require specific items.

### Files Created:
- `neko-atsume/cats.json` - Complete cat database with regular and rare cats
- `neko-atsume/toys.csv` - Toy/goodies data with costs and attractiveness ratings  
- `neko-atsume/game_config.yaml` - Game configuration and mechanics settings
- `neko-atsume/player_progress.txt` - Realistic player progress log example
- `neko-atsume/food_data.json` - Food types, costs, and feeding strategies
- `neko-atsume/test_scenarios.md` - 36 comprehensive test scenarios

**Key Data Points**: 
- 5 regular cats + 3 rare cats with detailed attributes
- 11 different toys with rarity levels and costs
- Complete feeding and currency systems
- Realistic player progression over 42 days

## 🏝️ Summer Pockets Reflection Blue Theme

**About**: Summer Pockets is an emotional visual novel by Key (creators of Clannad, Kanon, AIR) set on the remote island of Torishirojima. The Reflection Blue version adds new heroines and expanded storylines to the original game.

### Files Created:
- `summer-pockets/characters.json` - Complete character database with all heroines
- `summer-pockets/routes_config.yaml` - Story route structure and unlock conditions
- `summer-pockets/dialogue_samples.txt` - Authentic dialogue samples from various routes
- `summer-pockets/island_locations.csv` - All game locations with accessibility and atmosphere data
- `summer-pockets/music_tracks.json` - Comprehensive soundtrack information
- `summer-pockets/test_scenarios.md` - 60 detailed test scenarios

**Key Data Points**:
- 8 total heroines (4 original + 4 Reflection Blue additions)
- 10 story routes with 52+ hour total playtime
- 15 island locations with detailed descriptions
- 47 music tracks with emotional categorization

## 🧪 Testing Coverage

### File Format Variety:
- **JSON**: Structured data for characters, cats, food, music
- **CSV**: Tabular data for toys, locations  
- **YAML**: Configuration files for game settings and routes
- **TXT**: Progress logs and dialogue samples
- **MD**: Test scenarios and documentation

### Data Complexity Levels:
- **Simple**: Basic key-value pairs and lists
- **Nested**: Multi-level object hierarchies  
- **Arrays**: Collections of related objects
- **Mixed Types**: Combining strings, numbers, booleans, objects

### Testing Scenarios:
- **Neko Atsume**: 36 test scenarios covering functionality, edge cases, performance, UI/UX
- **Summer Pockets**: 60 test scenarios covering story routes, technical functionality, content validation

## 💡 Usage Ideas

These themed test files can be used for:
- **File Processing Tests**: Parsing different formats (JSON, CSV, YAML)
- **Data Validation**: Schema validation and data integrity checks  
- **Performance Testing**: Loading and processing various file sizes
- **Content Management**: Testing search, filter, and organization features
- **Localization Testing**: Character encoding and multilingual content
- **API Testing**: Using as mock data for endpoints
- **Database Testing**: Import/export functionality validation

Both themes provide rich, realistic data that goes beyond generic "Lorem ipsum" content, making tests more engaging and closer to real-world scenarios.