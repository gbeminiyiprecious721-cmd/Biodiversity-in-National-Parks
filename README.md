# Biodiversity in National Parks

## National Park Service Species Analysis

This project analyzes biodiversity data from the National Park Service to explore conservation patterns across species categories and national parks. The analysis focuses on conservation status, protection rates, endangered species trends, and species observation counts.

> **Note:** This dataset is inspired by real data but is largely fictional, so results should be interpreted as an educational analysis rather than a reflection of current ecological conditions.

## Project Goals

This project answers the following questions:

- What is the distribution of conservation status for species?
- Are certain categories of species more likely to be protected?
- Are differences between species category and conservation status statistically significant?
- Are certain categories more likely to be endangered?
- Which species are most prevalent, and how are they distributed across parks?

## Data Sources

The analysis uses two CSV files:

- `species_info.csv`: species-level information, including category, scientific name, common names, and conservation status.
- `observations.csv`: species observation counts across National Park Service parks.

## Analysis Overview

The project includes:

- Cleaning and preparing conservation status data.
- Comparing species categories by protection status.
- Calculating endangered rates by species category.
- Running a chi-square test to evaluate whether species category and conservation status are statistically associated.
- Identifying the most frequently observed species.
- Visualizing the distribution of the most observed species across national parks.

## Interpretation: Top 10 Most Observed Species

The top-10 most observed species chart highlights which species dominate total observations across the parks. This is useful for identifying common species in monitoring records and comparing the visibility of common species against protected or endangered species in the dataset.

## Key Findings

- Most species fall under `No Intervention`, while smaller groups are listed under protected conservation statuses.
- Protection rates vary by species category, suggesting some groups may be more at risk than others.
- Endangered rates also vary by category, with some categories showing a higher proportion of endangered species.
- A chi-square test was used to evaluate whether species category and conservation risk are associated. The p-value determines whether the relationship is statistically significant.
- The most observed species was identified, and its distribution across parks was visualized.

## Limitations

- The data is partially fictional and may not fully reflect real ecological conditions.
- Observation counts may be influenced by sampling effort, not only true species abundance.
- Endangered classifications are interpreted from available status labels and may not capture the full conservation context.

## Next Steps

- Compare conservation and endangered trends over time if temporal data becomes available.
- Analyze protected and endangered species specifically by park.
- Build a predictive model for conservation risk using species category and related features.

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

## How to Run

1. Clone this repository.
2. Add the dataset files to the project directory:
   - `species_info.csv`
   - `observations.csv`
3. Open the analysis notebook or Python script.
4. Run the cells or script to reproduce the cleaning, analysis, statistical testing, and visualizations.

## Conclusion

This project shows how biodiversity data can be used to explore conservation patterns across species categories and parks. While the dataset is mostly fictional, the workflow demonstrates practical data analysis techniques including grouping, visualization, proportion comparison, and statistical hypothesis testing.
