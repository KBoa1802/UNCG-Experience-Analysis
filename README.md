# UNCG College Experience Survey Analysis
This project analyzes student survey data from the University of North Carolina at Greensboro (UNCG) to examine whether certain demographic or academic variables influence how students rate various aspects of their college experience.

# Purpose
The goal of this project is to determine if factors such as Gender, Classification (e.g., Freshman, Sophomore), Race/Ethnicity, and Major have a significant effect on how students rate aspects of their experience at UNCG. Key areas of focus include:

Campus facilities and social life

Satisfaction with one's major

Affordability

Class and professor quality

Events and extracurriculars

Diversity and inclusion

Mental health resources

# Data
The data comes from a survey titled "College Experience Survey" and includes responses to Likert-style questions (1–10 scale) about different aspects of campus life.

Key Variables
Independent Variables: Gender, Classification, Race/Ethnicity, Major

Dependent Variables: Ratings for Mental Health, Campus, Professors, Classes, Affordability, Events, etc.

# Tools Used
R

Packages: dplyr, ggplot2, psych, stats

# Methodology
Data Cleaning: Removed irrelevant columns, converted key fields to factors.

Grouping & Aggregation: Used group_by() and summarise() to calculate average ratings across different demographic groups.

Visualization:

Bar plots and boxplots created using ggplot2 to visualize trends.

Group means displayed to enhance interpretability.

Statistical Modeling:

Linear models (lm()) were fitted to assess whether group membership significantly predicted specific ratings.

Example: MentalHealthRating ~ Gender

# Key Findings
Gender: No significant effect on mental health ratings.

Major: Media Studies students reported similar satisfaction levels as other majors.

Classification: Did not significantly affect ratings of professors or classes.

Race/Ethnicity: Aggregated and explored, but not extensively modeled in this version.

# File Structure
Code: Main R script for data processing, visualization, and modeling.

College Experience Survey (Responses).csv: Raw survey data (not included in repo for privacy).

README.md: This file.

# Notes
Due to potential sample size limitations (e.g., low counts in certain identity groups), interpretations should be made cautiously.

"Transgender" responses were excluded from some models due to low sample size but remain included in the raw data.

# Possible Extensions
Incorporate interaction terms in regression models.

Use more advanced models (e.g., logistic regression for binary outcomes).

Conduct significance testing across all demographic groups for more robust conclusions.

Explore qualitative responses if available.
