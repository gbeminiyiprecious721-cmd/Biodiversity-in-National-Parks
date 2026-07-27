# Biodiversity in National Parks

## National Park Service Species Analysis

This project analyzes biodiversity data from the National Park Service to explore conservation patterns across species categories and national parks. The analysis focuses on conservation status, protection rates, endangered species trends, and species observation counts.

> **Note:** This dataset is inspired by real data but is largely fictional, so results should be interpreted as an educational analysis rather than a reflection of current ecological conditions.

## What Problem This Solves

National parks track thousands of species, but raw biodiversity records can be difficult to interpret quickly. This project turns species and observation data into a clearer conservation overview by answering which species groups appear most at risk, which groups are most frequently observed, and whether conservation status is meaningfully associated with species category.

The goal is to help reviewers, analysts, and conservation-focused stakeholders understand biodiversity patterns faster through summary statistics, visualizations, and statistical testing.

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

## Example Workflow

The analysis follows a simple end-to-end data workflow:

1. **Input:** Load species records from `species_info.csv` and park observation records from `observations.csv`.
2. **Cleaning:** Replace missing conservation statuses with `No Intervention` and prepare category-level groupings.
3. **Processing:** Calculate conservation status counts, protection rates, endangered rates, and total observations by species.
4. **Statistical Testing:** Use a chi-square test to check whether species category and conservation status are associated.
5. **Result:** Generate charts and summary findings that show which species categories are most protected, most endangered, and most commonly observed.

Example output questions:

- Which species category has the highest protection rate?
- Which category has the highest endangered rate?
- What is the most observed species overall?
- How is the most observed species distributed across parks?

## Analysis Overview

The project includes:

- Cleaning and preparing conservation status data.
- Comparing species categories by protection status.
- Calculating endangered rates by species category.
- Running a chi-square test to evaluate whether species category and conservation status are statistically associated.
- Identifying the most frequently observed species.
- Visualizing the distribution of the most observed species across national parks.

## Visuals and Sample Outputs

Suggested visuals for this project include:

- Conservation status distribution chart.
- Protection rate by species category.
- Endangered rate by species category.
- Top 10 most observed species.
- Park-level distribution for the most observed species.

If chart images are exported from the notebook or script, they can be added to a repository folder such as `images/` and displayed like this:

![Top 10 Most Observed Species](images/top_10_species.png)
![Protection Rate by Category](images/protection_rate_by_category.png)
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

## Setup

Requirements
Python 3.8 or higher
Jupyter Notebook or another Python environment
pandas
NumPy
Matplotlib
Seaborn
SciPy

## Installation

Clone the repository:

git clone <repository-url>
cd <repository-folder>

Install dependencies:
pip install pandas numpy matplotlib seaborn scipy jupyter
Add the dataset files to the project directory:

species_info.csv
observations.csv

## How to Run

1. Clone this repository.
2. Add the dataset files to the project directory:
   - `species_info.csv`
   - `observations.csv`
3. Open the analysis notebook or Python script.
4. Run the cells or script to reproduce the cleaning, analysis, statistical testing, and visualizations.

## Conclusion

This project shows how biodiversity data can be used to explore conservation patterns across species categories and parks. While the dataset is mostly fictional, the workflow demonstrates practical data analysis techniques including grouping, visualization, proportion comparison, and statistical hypothesis testing.
