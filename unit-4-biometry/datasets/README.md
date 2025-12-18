\# Unit 4 Biometry Datasets



This folder contains real and simulated ecological datasets for practicing biometry concepts.



\## 📊 Available Datasets



\### 1. seed\_germination.csv

\*\*Description\*\*: Germination success rates for different plant species under various conditions.



\*\*Variables:\*\*

\- `species`: Plant species name

\- `temperature`: Temperature in °C

\- `light\_hours`: Hours of light per day

\- `seeds\_planted`: Number of seeds planted

\- `seeds\_germinated`: Number successfully germinated

\- `germination\_rate`: Proportion germinated



\*\*Distribution\*\*: Binomial  

\*\*Use for\*\*: Success/failure outcomes, proportions, chi-square test



---



\### 2. plant\_heights.csv

\*\*Description\*\*: Height measurements of adult plants in a population.



\*\*Variables:\*\*

\- `plant\_id`: Unique identifier

\- `species`: Plant species

\- `height\_cm`: Height in centimeters

\- `site`: Collection site

\- `light\_level`: Low, Medium, High



\*\*Distribution\*\*: Normal  

\*\*Use for\*\*: Central tendency (mean, median, mode), standard deviation, t-test



---



\### 3. species\_counts.csv

\*\*Description\*\*: Species counts across multiple sampling sites during succession.



\*\*Variables:\*\*

\- `site\_id`: Site identifier

\- `species\_name`: Species observed

\- `count`: Number of individuals

\- `habitat\_type`: Forest, Grassland, Wetland

\- `year`: Year of observation



\*\*Distribution\*\*: Poisson  

\*\*Use for\*\*: Rare events, species abundance patterns, diversity indices



---



\### 4. population\_samples.csv

\*\*Description\*\*: Population size estimates from different sampling methods.



\*\*Variables:\*\*

\- `sample\_id`: Sample number

\- `sampling\_method`: Random, Systematic, Stratified, Cluster

\- `estimated\_population`: Population estimate

\- `actual\_population`: True population (for comparison)

\- `sample\_size`: Number of individuals sampled

\- `habitat`: Sampling location



\*\*Use for\*\*: Comparing sampling techniques, sampling error, bias analysis



---



\### 5. treatment\_comparison.csv

\*\*Description\*\*: Plant growth under control vs. fertilizer treatment.



\*\*Variables:\*\*

\- `plant\_id`: Unique identifier

\- `treatment`: Control or Fertilizer

\- `height\_cm`: Final height after 8 weeks

\- `biomass\_g`: Dry biomass in grams

\- `leaf\_count`: Number of leaves



\*\*Use for\*\*: t-test, comparing two groups, hypothesis testing



---



\### 6. parasite\_load.csv \*(Coming Soon)\*

\*\*Description\*\*: Number of parasites per host organism.



\*\*Distribution\*\*: Negative Binomial  

\*\*Use for\*\*: Overdispersed/clumped distributions



---



\### 7. time\_to\_germination.csv \*(Coming Soon)\*

\*\*Description\*\*: Time in days for seeds to germinate under controlled conditions.



\*\*Distribution\*\*: Exponential  

\*\*Use for\*\*: Waiting time analysis, memoryless processes



---



\### 8. population\_sizes.csv \*(Coming Soon)\*

\*\*Description\*\*: Population sizes across multiple species in a community.



\*\*Distribution\*\*: Log-Normal  

\*\*Use for\*\*: Right-skewed distributions, multiplicative processes



---



\## 📁 Data Format



All datasets are in \*\*CSV (Comma-Separated Values)\*\* format, easily opened in:

\- Microsoft Excel

\- Google Sheets

\- Python (pandas)

\- R

\- Any text editor



\## 🔄 Using the Data



\### In Python:

```python

import pandas as pd

data = pd.read\_csv('seed\_germination.csv')

print(data.head())

```



\### In R:

```r

data <- read.csv('seed\_germination.csv')

head(data)

```



\### In Excel:

Just double-click the CSV file!



---



\## 🎲 Generating Synthetic Data



Need fresh data for teaching or practice? Use the scripts in `../scripts/data\_generators.py` (coming soon)



---



\## 📖 Citation



These datasets are created for educational purposes under CC BY 4.0 license.



If you use them in publications:

```

The Pattern Hunter Team. (2025). Unit 4 Biometry Educational Datasets. 

Interactive Ecology and Biometry Learning Platform.

https://github.com/The-Pattern-Hunter/interactive-ecology-biometry

```



---



\## 🤝 Contributing Datasets



Have real ecological data you'd like to share? 

\- Must be anonymized if from real research

\- Include proper metadata

\- Open an issue or pull request!



---



<div align="center">



\[🔙 Back to Unit 4](../)



</div>

