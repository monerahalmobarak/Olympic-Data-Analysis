# Olympic Data Analysis Project

## Overview
This project analyzes Olympic Games data using Python for data exploration and visualization. The dataset, sourced from Kaggle, provides historical insights into athletes, sports, and medal distributions, aiding in understanding patterns and trends over time.

---

## Dataset Details

The dataset contains 70,000 rows and includes the following key columns:
- **ID**: Unique identifier for each record.
- **Name**: Athlete's name.
- **Sex**: Athlete's gender.
- **Age**: Athlete's age at the event.
- **Height**: Athlete's height.
- **Weight**: Athlete's weight.
- **Team**: Team name.
- **NOC**: National Olympic Committee code.
- **Games**: Olympic Games year and season.
- **Year**: Year of the event.
- **Season**: Season of the event.
- **City**: Host city.
- **Sport**: Type of sport.
- **Event**: Specific event.
- **Medal**: Medal type (Gold, Silver, Bronze, or None).

---

## Data Preprocessing
1. **Cleaning Steps**:
   - Dropped the `ID` column as it was irrelevant for analysis.
   - Filled missing values in the `Medal` column with "No Medal."
   - Removed rows with missing values in `Age`, `Height`, and `Weight`.
   - Verified and removed duplicates.

2. **Outlier Removal**:
   - Used the Interquartile Range (IQR) method to detect and remove outliers from columns like `Year`, `Age`, `Height`, and `Weight`.
   - Visualized distributions with box plots before and after outlier removal.

---

## Data Exploration

### Key Visualizations:
1. **Histograms**:
   - Examined distributions of `Year`, `Age`, `Height`, and `Weight`.
   - Noted shifts in median height and weight over time, reflecting evolving athletic standards.

2. **Scatter Plots**:
   - Explored relationships between `Height` and `Weight`, segmented by gender.
   - Highlighted gender-based distinctions in physical attributes.

3. **Pair Plots**:
   - Investigated relationships among `Year`, `Age`, `Height`, `Weight`, and `Medal`.
   - Showed diverse profiles of medalists.

4. **Bar Charts**:
   - Medal distribution by sport, showing Athletics and Swimming as prominent.
   - Comparison of average `Age`, `Height`, and `Weight` by gender.

5. **Line Graphs**:
   - Tracked the average age of athletes over decades, noting fluctuations and a trend toward older ages in recent years.

6. **Geographical Visualizations**:
   - Used geomaps to display team locations and medal distributions globally.

---

## Data Visualization Tools
The project utilized the following libraries for interactive visualizations:
- **Plotly**: For creating dynamic plots like histograms, scatter plots, and 3D plots.
- **Matplotlib** and **Seaborn**: For static visualizations and statistical summaries.

---

## Key Insights
1. The average athlete age has risen over time, reflecting longer career spans.
2. Male athletes tend to have higher average height and weight than females.
3. Medal distribution is uneven, with a few sports dominating the tally.
4. Height and weight show a linear relationship, with gender-based distinctions.

---

## References
Kaggle Dataset: [Olympic Data](https://www.kaggle.com/datasets/bhanupratapbiswas/olympic-data)
