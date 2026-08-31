# Titanic Survival Analysis 🚢

A data analysis project exploring factors associated with passenger survival on the Titanic using Python, Pandas, and Matplotlib.

## Project Objective

The goal of this project is to clean and analyze the Titanic passenger dataset and investigate how characteristics such as passenger class, sex, age, and family size were associated with survival.

## Dataset

The project uses the Titanic dataset containing information about 891 passengers, including:

- Passenger class
- Sex
- Age
- Fare
- Number of siblings/spouses aboard
- Number of parents/children aboard
- Embarkation location
- Survival status

## Data Cleaning

The dataset contained several missing values. The following cleaning steps were performed:

- Removed the `deck` column because most of its values were missing.
- Filled missing `age` values using the median passenger age.
- Removed two records with missing embarkation information.
- Checked for duplicate-looking rows.
- Kept apparent duplicates because the dataset does not contain a unique passenger identifier.

After cleaning, the dataset contained 889 passenger records.

## Feature Engineering

Two new variables were created:

**Family Size**

Calculated using:

`family_size = sibsp + parch + 1`

**Age Group**

Passengers were divided into:

- Child
- Teen
- Young Adult
- Adult
- Senior

## Analysis

The project examined:

- Overall passenger survival rate
- Survival rate by passenger class
- Survival rate by sex
- Survival rate by age group
- Survival rate by family size

## Key Findings

- The overall survival rate was approximately 38%.
- First-class passengers had a substantially higher survival rate than third-class passengers.
- Female passengers had a much higher survival rate than male passengers.
- Children had the highest survival rate among the age groups analyzed.
- Passengers traveling with small families generally had higher survival rates than passengers traveling alone.
- Results for very large families should be interpreted carefully because those groups contained relatively few passengers.

## Visualizations

The project includes bar charts showing:

- Survival rate by passenger class
- Survival rate by sex
- Survival rate by age group
- Survival rate by family size

## Technologies Used

- Python
- Pandas
- Matplotlib
- Google Colab
- GitHub

## Skills Demonstrated

- Data loading and inspection
- Data cleaning
- Missing-value handling
- Duplicate analysis
- Feature engineering
- Pandas `groupby()`
- Exploratory data analysis
- Data visualization
- Interpretation of analytical results

## Notebook

See `Titanic_data_analysis.ipynb` for the complete analysis, code, outputs, and visualizations.
