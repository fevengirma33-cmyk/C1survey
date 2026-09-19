# Class 1 Survey Data Analysis

## Project Description
This repository contains the Class 1 survey dataset and the R Markdown code used to analyze it. The project is part of a course exercise to practice working with real-world survey data in R, including data inspection, cleaning, recoding, and basic descriptive statistics.

## Files Included
- `c1survey.csv`: The Class 1 survey dataset 
- `class1_survey_analysis.Rmd`: The R Markdown file containing the analysis code
- `README.md`: This file

## About the Dataset
The Class 1 survey dataset contains responses collected from students, including variables such as birth day (`bday`) and birth month (`bmonth`), among others. Variables include a mix of numeric and character types. The raw data contained some unusual or inconsistently entered values (for example, month names entered as text and a malformed date entry), which are addressed in the cleaning steps.

## What the Code Does
- Reads in the survey dataset
- Counts the number of factor, integer, numeric, and character variables
- Checks the `bday` and `bmonth` variables for unusual or missing values using the `table()` function
- Cleans unusual values (recodes text month names to numbers, sets an invalid entry to NA) and converts variables to numeric
- Calculates the median birth day and birth month
- Creates a new variable, `bseason`, assigning each respondent to a meteorological season based on birth month
- Produces a cross-tabulation and uses `addmargins()` to count how many classmates were born in each season
- Explores an additional question of interest using the survey variables

## How to Run the Code
1. Download or clone this repository to your computer
2. Open the `.Rmd` file in RStudio
3. Make sure the dataset is in the same folder and your working directory is set to that folder
4. Run the code chunks (or knit the document)

## Author
- Name: Feven Taye
