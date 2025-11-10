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


##  Objectives

1. Identify the overall top five baby names and classify them as *Classic* or *Trendy*.  
2. Find the top 20 male names and determine where “Paul” ranks among them.  
3. Discover female names appearing in both 1920 and 2020, showing long-term popularity.
## SQL Techniques Used

| Technique | Purpose |
|------------|----------|
| **Common Table Expressions (CTEs)** | Simplify multi-step logic and reuse subquery results |
| **Aggregate Functions** (`SUM`, `COUNT`) | Compute total occurrences per name |
| **Window Functions** (`RANK() OVER`) | Rank male names by total popularity |
| **Conditional Logic** (`CASE WHEN`) | Classify names as *Classic* or *Trendy* |
| **Self-Joins** | Compare female names between 1920 and 2020 |
| **Filtering & Sorting** (`WHERE`, `ORDER BY`, `LIMIT`) | Extract focused and readable result sets |

###  1.Top Five Names (Classic vs. Trendy)

*Query available in **1️ Top Five Names (Classic vs. Trendy)**
*Full SQL query available in [`notebook (1).ipynb`](notebook%20(1).ipynb)*
**Insight:**
This query highlights the most enduring names across a century. *Classic* names show consistent use, while *Trendy* names surge briefly and fade.

### 2. Top 20 Male Names & Rank of “Paul”**
*Full SQL query available in [`notebook (1).ipynb`](notebook%20(1).ipynb)*
**Insight:**
This ranking reveals traditional male names that have dominated over time. The position of **“Paul”** shows how some names maintain modest popularity compared to cultural icons like *James* or *John*.
### 3. Female Names Appearing in Both 1920 and 2020**
*Full SQL query available in [`notebook (1).ipynb`](notebook%20(1).ipynb)*
**Insight:**
This identifies names with remarkable longevity. Names like *Mary*, *Elizabeth*, and *Anna* appear in both years, reflecting enduring cross-generational appeal.

## Key Insights

* **Classic names** (e.g., James, Mary, John) have persisted for decades, reflecting cultural stability.
* **Trendy names** emerge and fade quickly, often tied to pop culture or famous personalities.
* **Male names** tend to remain popular longer, while **female names** show faster trend cycles.
* The dataset showcases the **power of SQL** in extracting cultural and demographic patterns through data.

## Tools & Environment

* **Database:** PostgreSQL
* **Interface:** Jupyter Notebook (`ipython-sql` extension)

##  Conclusion
This PostgreSQL project demonstrates how SQL can be used for data storytelling and historical insight.
By combining analytical techniques like CTEs, window functions, and joins, it uncovers how American naming culture evolved over a century ,balancing tradition and trend.







