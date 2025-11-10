# Exploring-Trends-In-American-Baby-Names

## Overview
This project analyzes historical trends in baby names in the United States between 1920 and 2020 using PostgreSQL.  
The goal is to uncover long-term naming patterns, identify names that have remained popular over time, and highlight how social and cultural changes influence naming preferences.

The analysis was performed entirely in PostgreSQL, with queries executed through Jupyter Notebook using the `ipython-sql` extension.

##  Dataset Information

Source: [U.S. Social Security Administration (SSA)](https://www.ssa.gov/oact/babynames/)  
Description:Contains all first names given to babies in the U.S. for each year, along with gender and number of registered births.  
Period Covered: 1920 – 2020  


| Column | Type | Description |
|---------|------|-------------|
| `year` | INTEGER | Year of record |
| `first_name` | VARCHAR | Baby’s first name |
| `sex` | VARCHAR | Gender of the baby (`M` or `F`) |
| `num` | INTEGER | Number of babies registered with that name |

