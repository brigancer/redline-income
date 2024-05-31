# DRAFT written by AI

# Redlining and Socioeconomic Disparities in Davidson County

This repository explores the relationship between historical redlining practices and socioeconomic disparities in Davidson County. We leverage census data, historical redlining maps, and geospatial analysis to investigate the impact of redlining on income distribution, household counts, and spatial patterns.

## Project Workflow

1.  **Data Collection and Preparation:**

    *   **Redlining Data:**
        *   Source: Historical Redlining Maps (HRI) and University of Richmond Mapping Inequality Data
        *   Format: Shapefiles (HRI) and GeoJSON (University of Richmond)
        *   Processing: Filtering for Davidson County, renaming columns for consistency.
    *   **Census Income Data:**
        *   Source: U.S. Census Bureau (2000, 2010, 2020)
        *   Format: CSV files
        *   Processing:
            *   Selecting relevant columns (income levels, household counts, etc.)
            *   Calculating income counts from percentages (2010 and 2020 data)
            *   Cleaning and standardizing tract IDs
            *   Joining census data with redlining data

2.  **Exploratory Data Analysis (EDA):**

    *   **Analysis Notebooks:** `redlining_eda.Rmd`
    *   **Goals:**
        *   Examine income distribution across different redlining grades (using income percentages and counts).
        *   Visualize changes in income distribution over time (2000-2020).
        *   Explore relationships between redlining scores and household income (median and mean).

3.  **Geospatial Analysis:**

    *   **Analysis Notebook:** `redlining_geospatial.Rmd`
    *   **Goals:**
        *   Map historical redlining grades for Davidson County.
        *   Visualize spatial patterns of income distribution in relation to redlining grades.
        *   Compare redlining boundaries from different data sources (HRI and University of Richmond).

## Key Questions

*   How does historical redlining correlate with income levels in different areas of Davidson County?
*   Have income disparities changed over time (2000-2020) in historically redlined areas?
*   Are there spatial patterns in the distribution of income and redlining grades?
*   How do redlining boundaries from different data sources compare?

## Repository Contents

*   `/data/`: Contains the raw and processed data files.
*   `redlining_eda.Rmd`: R Markdown notebook for EDA.
*   `redlining_geospatial.Rmd`: R Markdown notebook for geospatial analysis.
*   `README.md`: This file.

## How to Use This Repository

1.  **Clone:** Clone this repository to your local machine.
2.  **Data:** Ensure the data files are in the correct subdirectories within `/data/`.
3.  **Run Analysis:** Open and execute the R Markdown notebooks (`redlining_eda.Rmd` and `redlining_geospatial.Rmd`) in RStudio.

## Future Work

*   Expand analysis to include additional socioeconomic factors (housing, education, race).
*   Perform more robust statistical analyses (e.g., regression modeling).
*   Incorporate interactive maps and visualizations for a deeper understanding of spatial patterns.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

## License

This project is licensed under the MIT License.
