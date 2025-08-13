# 🌱 Stardew Valley Theme Test Data

**About**: Stardew Valley is a beloved indie farming simulation game created by ConcernedApe. Players inherit their grandfather's old farm and work to restore it while building relationships with townspeople, exploring caves, and participating in seasonal festivals.

This theme provides comprehensive test data covering the core gameplay systems: farming, social relationships, crafting, seasonal events, and player progression.

---

## 📁 Files Overview

### `crops.json` - Seasonal Farming Database (200+ lines)
**Format**: JSON  
**Content**: Complete crop database with seasonal farming data

**Key Features**:
- **12 crops** across 4 seasons with detailed agricultural stats
- **Economic data**: Seed costs, sell prices, profit-per-day calculations
- **Growth mechanics**: Days to maturity, regrowth patterns, fertilizer effects
- **Quality systems**: Normal/Silver/Gold/Iridium quality multipliers
- **Special features**: Giant crops, artisan processing, desert exclusives

**Data Structure**:
```json
{
  "metadata": { "version", "theme", "description" },
  "seasons": {
    "spring/summer/fall/winter": {
      "crops": [
        {
          "id", "name", "seed_price", "sell_price", 
          "growth_days", "regrows", "quality_multipliers",
          "profit_per_day", "difficulty", "special_features"
        }
      ]
    }
  },
  "fertilizers": [...],
  "farming_stats": {...}
}
```

### `villagers.csv` - Relationship & Social Data (30 villagers)
**Format**: CSV  
**Content**: Complete villager database with relationship mechanics

**Key Features**:
- **30 unique NPCs** with detailed personal information
- **Gift systems**: Loved/liked/neutral/disliked/hated items for each villager
- **Demographics**: Ages, occupations, relationships, birthdays, personalities
- **Daily schedules**: Morning, afternoon, evening location patterns
- **Marriage system**: 12 marriage candidates with special mechanics
- **Social dynamics**: Complex relationship webs and community interactions

**Columns**: `name`, `age`, `gender`, `occupation`, `location`, `relationship_status`, `birthday_season`, `birthday_day`, `heart_level_max`, `loved_gifts`, `liked_gifts`, `neutral_gifts`, `disliked_gifts`, `hated_gifts`, `schedule_*`, `marriage_candidate`, `personality_type`, `hobby`

### `items_database.yaml` - Crafting & Economics (150+ items)
**Format**: YAML  
**Content**: Comprehensive item database with crafting and economic systems

**Key Features**:
- **6 major categories**: Crops, Artisan Goods, Mining, Fishing, Foraging, Crafting
- **Economic systems**: Sell prices, processing times, profit calculations
- **Crafting recipes**: Materials, unlock conditions, recipe sources
- **Artisan processing**: Wine/cheese/mayo production with aging mechanics
- **Mining data**: Ores, gems, smelting systems, legendary items
- **Bundle systems**: Community Center requirements and rewards

**Structure**: Hierarchical YAML with nested categories, recipes, and economic data

### `seasonal_events.json` - Calendar & Festivals (8+ events)
**Format**: JSON  
**Content**: Complete festival calendar with detailed event mechanics

**Key Features**:
- **8 major festivals** distributed across all seasons
- **Competition systems**: Egg hunt, grange display, ice fishing contests
- **Social mechanics**: Gift exchanges, community interactions
- **Seasonal effects**: Weather patterns, special mechanics per season
- **Reward systems**: Festival shops, unique items, relationship bonuses
- **Special events**: Cutscenes, weather events, magical occurrences

**Coverage**: Spring (1), Summer (2), Fall (2), Winter (2), Plus special events

### `farm_progress.txt` - Player Journey Log (112 days)
**Format**: Plain Text  
**Content**: Realistic player progression through first year

**Key Features**:
- **Full year timeline**: Day-by-day progression through Year 1
- **Financial tracking**: Income, expenses, ROI analysis, net worth progression
- **Skill development**: All 5 skills with realistic level progression
- **Relationship building**: Multi-character relationship arcs over time
- **Achievement system**: Unlocks, milestones, completion tracking
- **Strategic decisions**: Crop choices, building priorities, optimization

**Format**: Chronological log with seasonal summaries and performance metrics

### `test_scenarios.md` - Testing Documentation (72 scenarios)
**Format**: Markdown  
**Content**: Comprehensive testing scenarios covering all data types

**Coverage**:
- **72 detailed scenarios** across 6 major testing categories
- **Complexity levels**: Basic (25), Intermediate (30), Advanced (17)
- **Testing types**: Functionality (35), Validation (15), Performance (12), Integration (10)
- **Cross-file integration**: Multi-format testing scenarios
- **Real-world applications**: Game development, data processing, economic modeling

---

## 🎯 Key Data Points

### Agricultural Systems
- **12 unique crops** with seasonal availability
- **4 seasons** with distinct growing patterns
- **5 difficulty levels** from beginner to legendary
- **Complex economics**: Seed costs, growth times, profit optimization
- **Processing chains**: Raw crops → Artisan goods → Aged products

### Social Systems  
- **30 unique NPCs** with individual personalities and preferences
- **12 marriage candidates** with special romance mechanics
- **Gift preferences**: 5 categories per villager (loved/liked/neutral/disliked/hated)
- **Daily schedules**: 3 time periods with location tracking
- **Community events**: 8 festivals with social interaction opportunities

### Economic Complexity
- **150+ items** across 6 major categories
- **85 craftable items** with material requirements
- **Multi-tier processing**: Raw materials → Refined goods → Artisan products
- **Market dynamics**: Seasonal pricing, festival shops, bundle requirements
- **Optimization puzzles**: Profit maximization, resource allocation

### Temporal Systems
- **112-day year cycle** with seasonal mechanics
- **8 major festivals** with specific dates and activities
- **Weather patterns**: Seasonal effects, special events, random occurrences
- **Long-term progression**: Multi-year planning, achievement systems

---

## 💡 Testing Applications

### Data Processing Tests
- **JSON parsing**: Complex nested structures with arrays and objects
- **CSV handling**: Large tabular data with complex string parsing
- **YAML processing**: Hierarchical configuration-style data
- **Text mining**: Unstructured log data extraction and analysis

### Economic Modeling
- **Profit optimization**: Multi-variable economic calculations
- **Resource allocation**: Limited resource optimization problems
- **Market simulation**: Supply/demand dynamics, pricing models
- **Investment analysis**: ROI calculations, risk assessment

### Social Network Analysis
- **Relationship mapping**: Complex interpersonal networks
- **Preference modeling**: Multi-dimensional preference systems
- **Community dynamics**: Group behavior, event participation
- **Influence propagation**: How relationships affect game outcomes

### Temporal Data Analysis
- **Seasonal patterns**: Cyclical data analysis, trend detection
- **Event scheduling**: Complex calendar systems, conflict resolution
- **Progression tracking**: Longitudinal data analysis, milestone detection
- **Performance optimization**: Time-series analysis of player efficiency

### Game Development Testing
- **Balance validation**: Economic systems, difficulty curves
- **Content verification**: Asset completeness, reference integrity
- **Performance testing**: Large dataset processing, query optimization
- **Integration testing**: Multi-system interactions, data consistency

---

## 🚀 Usage Examples

### Basic Queries
```
- Filter crops by season and profitability
- Find villagers by gift preferences and birthday
- Calculate artisan good processing chains
- Extract festival dates and requirements
```

### Complex Analysis
```
- Optimize year-long crop rotation for maximum profit
- Generate personalized gift recommendations for all villagers
- Model Community Center bundle completion strategies
- Analyze festival participation for relationship optimization
```

### Performance Testing
```
- Process 30-villager relationship matrix efficiently
- Handle complex multi-level YAML structure navigation
- Parse chronological progression data for trend analysis
- Execute cross-format data validation across all files
```

### Integration Scenarios
```
- Cross-reference crop data with festival requirements
- Validate villager gift preferences against item database
- Synchronize seasonal mechanics across all data sources
- Build comprehensive farm planning tools using all datasets
```

---

## 📊 Statistics

- **Total Data Files**: 6 files across 4 formats
- **Total Content**: 800+ lines of structured data
- **Testing Coverage**: 72 comprehensive scenarios
- **Data Complexity**: Simple key-values to complex nested hierarchies
- **Cross-References**: Multiple inter-file data relationships
- **Real-World Accuracy**: Based on actual game mechanics and content

---

## 🌟 Why This Theme Works for Testing

**Rich Data Relationships**: Unlike simple test data, these files contain realistic cross-references and dependencies that mirror real-world applications.

**Multiple Complexity Levels**: From basic data parsing to complex economic optimization, supporting tests for different skill levels and use cases.

**Diverse Formats**: JSON, CSV, YAML, and plain text provide comprehensive format coverage for file processing tests.

**Engaging Content**: Farm simulation data is more interesting than Lorem ipsum, making tests more engaging and memorable.

**Realistic Scale**: Data volumes and complexity match real-world applications, providing meaningful performance benchmarks.

**Community Connection**: Stardew Valley's popularity means many testers will recognize and understand the data context.

This theme transforms mundane testing scenarios into engaging puzzles involving crop optimization, relationship building, and economic strategy - making the testing process both educational and enjoyable.