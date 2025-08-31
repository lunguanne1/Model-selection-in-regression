# Movie Popularity Analysis – Regression Models

This repository contains a project for the **Regression Models** course (2025), focusing on model selection and applied regression using R.  
The main goal is to analyze the factors that influence a movie’s popularity and to evaluate which regression models best explain IMDb ratings.

## Authors
- Daria Cristiana Țăranu 
- Anne-Marie Lungu  

## Contents
- `Proiect filme.Rmd` – R Markdown file with code, analysis, and visualizations  
- `movies.csv` – dataset with 750 movies, including title, year, genre, IMDb rating, Metacritic score, votes, and gross earnings  
- `Proiect Modele de Regresie 2025.pdf` – final project report (in Romanian)  

## Methodology
- **Exploratory Data Analysis (EDA):** distribution of genres, ratings, scores, votes, and gross earnings  
- **Correlation analysis:** IMDb rating vs. Meta_score, No_of_Votes, Gross  
- **Simple regression models:** one predictor at a time  
- **Multiple regression models:** combinations of predictors (Meta_score, No_of_Votes, Gross)  
- **Interaction models:** tested interactions between predictors  
- **Model selection:** evaluation based on R², AIC, and BIC  

## Key Findings
- IMDb ratings are positively correlated with both **Meta_score** and **No_of_Votes**  
- Gross earnings show only a weak relationship with IMDb ratings  
- The best models are those combining **Meta_score** and **No_of_Votes**, explaining ~45% of the variation  
- Adding **Gross** as a predictor slightly improves performance (R² ≈ 0.51)  
- AIC favored a model with interactions, while BIC preferred a simpler model with three predictors  

## How to run
Open `Proiect filme.Rmd` in RStudio and knit the file to reproduce the full analysis.  
Required packages:  
```R
install.packages(c("tidyverse", "GGally", "ggplot2"))
