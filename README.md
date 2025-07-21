
# A/B Testing Analysis

This project analyzes marketing campaign performance using A/B testing. It visualizes the user conversion flow using a Sankey diagram built with Plotly, highlighting the path from the marketing source (ad or PSA) to the final conversion status (converted or not), segmented by the day of the week.


## Files Included

- ```marketing_AB.csv:``` Dataset containing user interaction data.

- ```testing.ipynb:``` Jupyter Notebook with data preprocessing, analysis, and visualization code.

- ```figure_35.html:``` Interactive Sankey diagram showing conversion flow.

- ```conversion.png:``` Image snapshot of the Sankey diagram.


## Tools & Libraries


- Python

- Pandas – for data cleaning and manipulation

- Plotly – for interactive Sankey diagram visualization

- Jupyter Notebook


## Analysis Goals
- Compare the performance of ad vs psa campaigns.

- Understand which day of the week results in higher conversions.

- Visualize the user journey from source to conversion outcome.
## Key Steps in the Analysis

### 1. Data Loading
- Read ```marketing_AB.csv``` to explore test groups, dates, and conversion labels.

### 2. Preprocessing

- Extract day of the week from timestamps.

- Normalize test group names (e.g., ad, psa).

- Group and count conversions across dimensions.

### 3. Sankey Diagram Construction

- Nodes represent stages (e.g., source, weekday, conversion status).

- Links represent user flows between stages.

- Visualized using Plotly and exported as HTML.

``` bash
Source (ad/psa) → Day (Monday–Sunday) → Outcome (Converted/Not Converted)

```

![conversion Flow](https://github.com/KomalGangwar/A-B_testing_analysis/blob/1eb77603bda56c1962d09b09de6f13e1cd5c9c7b/iframe_figures/conversion.png)

## Insights

- The ad group drives the majority of traffic.

- Most conversions occur on specific weekdays (visible in Sankey thickness).

- PSA campaigns have lower engagement and conversion rates.
## How to Run

  Clone the repo:

```bash
git clone https://github.com/KomalGangwar/A-B_testing_analysis.git
cd A-B_testing_analysis

```

Install dependencies:

```bash
pip install pandas plotly notebook

```
Open and run:

```bash
jupyter notebook testing.ipynb

```
## Author

- [Komal Gangwar](https://github.com/KomalGangwar)

