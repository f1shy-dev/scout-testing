# Stardew Valley Test Scenarios

**Theme**: Stardew Valley Farming Simulation
**Total Scenarios**: 72
**Data Coverage**: Crops, Villagers, Items, Events, Farm Progression
**File Formats**: JSON, CSV, YAML, TXT, MD

---

## 📊 Crop Data Testing (crops.json) - 18 scenarios

### Functionality Testing
1. **Seasonal Crop Filtering**: Filter crops by season (spring/summer/fall/winter) and validate seasonal availability
2. **Profit Calculation**: Calculate profit per day for each crop using sell_price, seed_price, and growth_days
3. **Quality Multiplier Application**: Apply quality multipliers (normal/silver/gold/iridium) to base crop values
4. **Regrowth Crop Identification**: Identify all crops with regrows property and calculate continuous harvest profits
5. **Giant Crop Detection**: Find all crops that can become giant crops and validate their special properties
6. **Artisan Processing Chain**: Map crops to their artisan products (wine, jam, etc.) and calculate value increases
7. **Fertilizer Impact Calculation**: Apply fertilizer effects to crop growth times and quality chances
8. **Seasonal Statistics Aggregation**: Calculate total crops per season and difficulty distribution

### Edge Cases
9. **Winter Crop Limitations**: Handle limited winter crop availability and greenhouse alternatives
10. **Cross-Season Crops**: Validate crops like coffee beans that span multiple seasons
11. **Desert-Only Crops**: Handle special location requirements for crops like starfruit
12. **Quality Scaling Boundaries**: Test quality multipliers at maximum (iridium) and minimum (normal) values
13. **Zero Profit Crops**: Handle edge cases where seed cost exceeds sell price
14. **Missing Data Handling**: Gracefully handle crops without regrowth or artisan product data

### Performance Testing
15. **Large Crop Dataset**: Process entire crop database efficiently for complex filtering operations
16. **Profit Optimization**: Calculate optimal crop combinations for maximum profit across seasons
17. **Multi-Season Planning**: Process year-long farming strategies with crop rotation analysis

### Integration Testing
18. **Cross-Reference Validation**: Verify crop data consistency with items_database.yaml and seasonal_events.json

---

## 👥 Villager Relationship Testing (villagers.csv) - 15 scenarios

### Functionality Testing
19. **Gift Preference Matching**: Match loved/liked gifts to villager preferences for relationship building
20. **Marriage Candidate Filtering**: Identify all marriage-eligible villagers and their requirements
21. **Birthday Calendar Generation**: Create calendar view of all villager birthdays by season
22. **Age Demographics Analysis**: Analyze villager age distribution and demographic patterns
23. **Occupation-Based Grouping**: Group villagers by occupation and location for community analysis
24. **Schedule Pattern Analysis**: Parse daily schedules to understand villager movement patterns
25. **Friendship Level Tracking**: Process heart levels and relationship progression for multiple villagers

### Data Validation
26. **Gift List Parsing**: Parse complex gift lists with semicolon separators and handle special cases
27. **Schedule Format Validation**: Validate schedule location format consistency across all villagers
28. **Relationship Status Verification**: Cross-check marriage candidates with relationship status data
29. **Location Reference Validation**: Ensure all schedule locations reference valid game locations

### Performance Testing
30. **Gift Recommendation Engine**: Generate optimal gift recommendations for multiple villagers efficiently
31. **Complex Query Processing**: Handle complex filtering combining age, location, marriage status, and preferences
32. **Large Dataset Relationship Mapping**: Process relationship networks and friendship webs efficiently

### Edge Cases
33. **Universal Gift Handling**: Process "Universal Loves" and special gift categories correctly

---

## 🛠️ Items Database Testing (items_database.yaml) - 12 scenarios

### Functionality Testing
34. **Crafting Recipe Validation**: Parse crafting recipes and validate ingredient requirements
35. **Economic Analysis**: Calculate profit margins for artisan goods processing chains
36. **Mining Resource Mapping**: Map ores to their smelted products and processing times
37. **Fishing Data Processing**: Process fish data including seasons, locations, and difficulty ratings
38. **Bundle Requirement Matching**: Match items to Community Center bundle requirements
39. **Artisan Machine Recipes**: Parse complex artisan machine crafting requirements

### Performance Testing
40. **Large Item Database Queries**: Efficiently search and filter across 150+ items
41. **Complex Recipe Calculations**: Calculate multi-step processing chains for maximum profit
42. **Seasonal Availability Mapping**: Process seasonal item availability across all categories

### Data Structure Testing
43. **YAML Hierarchy Navigation**: Navigate complex nested YAML structure efficiently
44. **Multi-Type Data Handling**: Process mixed data types (strings, arrays, objects) in single queries
45. **Cross-Category References**: Handle references between different item categories

---

## 🎉 Seasonal Events Testing (seasonal_events.json) - 9 scenarios

### Event Logic Testing
46. **Festival Date Calculation**: Calculate exact festival dates and validate seasonal distribution
47. **Competition Scoring**: Implement grange display scoring system with category and quality bonuses  
48. **Gift Exchange Logic**: Handle random gift assignment for Feast of Winter Star
49. **Weather Event Triggers**: Process random weather events and their effects
50. **Festival Shop Processing**: Handle limited-time festival shop items and pricing

### Data Consistency
51. **Calendar Integration**: Ensure festival dates don't conflict with other seasonal mechanics
52. **Reward System Validation**: Validate festival rewards and their in-game value
53. **NPC Participation**: Cross-reference festival attendance with villager data
54. **Seasonal Mechanics**: Validate seasonal weather patterns and their game effects

---

## 📈 Farm Progress Testing (farm_progress.txt) - 9 scenarios

### Progress Tracking
55. **Timeline Parsing**: Parse chronological farm progress entries and calculate time spans
56. **Financial Analysis**: Track income progression and calculate ROI for different strategies
57. **Skill Progression Validation**: Validate skill level progression follows game mechanics
58. **Relationship Timeline**: Track friendship progression with multiple villagers over time
59. **Achievement Tracking**: Monitor achievement unlock progression and completion rates

### Data Mining
60. **Efficiency Analysis**: Analyze farming strategies and identify optimization opportunities
61. **Seasonal Performance**: Compare performance metrics across different seasons
62. **Goal Achievement Tracking**: Monitor progress toward long-term objectives
63. **Resource Management**: Analyze resource allocation and inventory management strategies

---

## 🔄 Cross-File Integration Testing - 9 scenarios

### Data Consistency
64. **Price Validation**: Verify consistent pricing between crops.json and items_database.yaml
65. **Villager Gift Cross-Reference**: Match villager loved gifts with available items in database
66. **Festival Item Availability**: Ensure festival rewards exist in main items database
67. **Seasonal Crop Validation**: Cross-check seasonal crop availability with event calendar
68. **Recipe Ingredient Verification**: Verify all crafting recipe ingredients exist in items database

### Complex Scenarios
69. **Annual Profit Optimization**: Use all data sources to calculate optimal year-long strategy
70. **Community Center Completion**: Track bundle progress using items from multiple data sources
71. **Villager Relationship Optimization**: Use gift data, birthday calendar, and festival events for relationship building
72. **Complete Farm Planning**: Integrate crops, events, villagers, and progression data for comprehensive farm planning

---

## 🎯 Testing Categories Summary

### By Complexity Level
- **Basic**: 25 scenarios (data parsing, simple queries, validation)
- **Intermediate**: 30 scenarios (calculations, filtering, cross-referencing) 
- **Advanced**: 17 scenarios (optimization, complex integrations, performance testing)

### By Testing Type
- **Functionality**: 35 scenarios
- **Data Validation**: 15 scenarios
- **Performance**: 12 scenarios
- **Integration**: 10 scenarios

### By File Format
- **JSON Testing**: 27 scenarios (crops.json, seasonal_events.json)
- **CSV Testing**: 15 scenarios (villagers.csv)
- **YAML Testing**: 12 scenarios (items_database.yaml)
- **Text Processing**: 9 scenarios (farm_progress.txt)
- **Cross-Format**: 9 scenarios (multi-file integration)

---

## 💡 Usage Examples

### Data Processing Pipeline
```
1. Load crop data → Filter by season → Calculate profits → Rank by efficiency
2. Load villager data → Parse gift preferences → Match with item database → Generate recommendations
3. Load event calendar → Extract festival dates → Cross-reference with villager schedules → Plan optimal socializing
4. Parse farm progress → Extract financial data → Calculate growth rates → Identify successful strategies
```

### Complex Query Examples
```
- "Find the most profitable spring crops that can be processed into artisan goods"
- "Generate gift recommendations for all marriage candidates based on their preferences and birthdays"
- "Calculate optimal festival participation strategy for maximum profit and relationship building"
- "Analyze farm progression patterns to identify key success milestones"
```

### Testing Automation
```
- Automated data validation across all JSON/CSV/YAML files
- Performance benchmarking for complex queries and calculations
- Integration testing between related data structures
- Regression testing for data consistency after updates
```

---

**Note**: These scenarios provide comprehensive testing coverage for a farming simulation game theme, offering realistic data structures and complex relationships typical of actual game development and data processing needs.