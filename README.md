# Hong Kong Temperature Visualization

## Overview
This project visualizes daily temperature data for Hong Kong using D3.js on Observable. The visualization consists of two levels of complexity:
1. A Year/Month Heatmap showing monthly temperature patterns across years
2. An enhanced version that includes daily temperature variations within each month-year cell

## Data
The visualization uses `temperature_daily.csv`, which contains daily temperature records for Hong Kong over multiple years.

![Data Table Sample](path/to/data_table_image.png)
*Figure 1: Sample of the temperature data in tabular format*

## Level 1: Year/Month Heatmap
This visualization presents a matrix view where:
- X-axis represents years
- Y-axis represents months
- Each cell is colored according to the temperature value for that month-year combination

### Features
- Toggle between maximum and minimum temperature views
- Hover tooltips showing date and exact temperature values
- Color legend indicating the temperature scale
- Clear visual pattern of seasonal temperature changes across years

### Interaction
- Click the buttons to switch between maximum and minimum temperature views
- Hover over any cell to see detailed information

![Level 1 Maximum Temperature Heatmap](path/to/level1_max_temp.png)
*Figure 2: Level 1 visualization showing maximum temperatures by month and year*

![Level 1 Minimum Temperature Heatmap](path/to/level1_min_temp.png)
*Figure 3: Level 1 visualization showing minimum temperatures by month and year*

## Level 2: Enhanced Heatmap with Daily Temperature Variations
This advanced visualization builds on Level 1 by adding:
- Mini line charts inside each month-year cell showing daily temperature fluctuations
- Focus on the most recent 5-10 years for better readability
- Preservation of the color-coding system from Level 1

### Features
- All Level 1 features plus:
- Daily temperature trends visible within each month
- Ability to identify extreme temperature days within months
- Clearer visualization of weather patterns and anomalies

### Implementation Details
- Each cell contains a small multiples chart showing day-by-day temperature changes
- X-axis of mini-charts represents days (1-31)
- Y-axis of mini-charts represents temperature values
- Consistent color scheme throughout for easy interpretation

![Level 2 Maximum Temperature Visualization](path/to/level2_max_temp.png)
*Figure 4: Level 2 visualization showing daily maximum temperature variations within each month-year cell*

![Level 2 Minimum Temperature Visualization](path/to/level2_min_temp.png)
*Figure 5: Level 2 visualization showing daily minimum temperature variations within each month-year cell*

## Usage Instructions
1. Visit the Observable notebook at the provided URL
2. The default view shows the Level 1 heatmap with maximum temperatures
3. Use the toggle buttons to switch between viewing maximum and minimum temperatures
4. Hover over cells to see specific temperature information
5. Scroll down to view the Level 2 visualization with daily temperature variations
6. The color legend helps interpret temperature values across all visualizations

## Technical Implementation
The visualization is built using:
- D3.js for data binding and visualization
- Observable's reactive notebook environment
- SVG for rendering the heatmaps and line charts
- JavaScript for interaction handling

## Analysis Insights
This visualization effectively reveals:
- Seasonal temperature patterns in Hong Kong
- Year-to-year temperature trends and potential climate change indicators
- Unusual temperature events or anomalies
- Day-to-day temperature volatility within months
