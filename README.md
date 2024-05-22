# USA States Sustainability Clustering Study

This repository contains the paper, code, and data for the paper titled "Fuzzy Clustering with Hierarchical Agglomerative Clustering for Applications in Sustainability." The project aims to establish a data-driven approach to develop sustainability policies at the state level in the United States using fuzzy and hierarchical clustering techniques.

This project was completed as part of CS 4824: Machine Learning at Virginia Tech, under the guidance of Dr. Dawei Zhou.

## Quick Links
- [Replication Data for: Fuzzy Clustering with Hierarchical Agglomerative Clustering for Applications in Sustainability](./data/Final.csv)
- [Link to Project Proposal](./Project%20Proposal.pdf)
- [Link to Final Presentation](./Final_Slides.pdf)
- [Link to Final Paper](./Final_Report.pdf)
- [Link to Code](./src/model/FINAL_MODELS.ipynb)

## Features
- Explore fuzzy clustering and hierarchical agglomerative clustering for sustainability policy development.
- Analyze state-level sustainability using an entropy-based weighting metric for nuanced clustering.
- Visualize complex state relationships through customized dendrograms.

## Milestones

**Data Collection**
   - Utilized the DPSIR Framework for comprehensive state-specific sustainability metric collection.
   - Integrated diverse data sources (EPA, EIA, US Census Bureau) on energy consumption, carbon emissions, demographics, and socio-economics.

**Data Preprocessing**
   - Cleaned, normalized, and transformed collected data for consistency.
   - Applied entropy-based methods to handle data variability and assess metric significance.

**Feature Selection/Extraction**
   - Implemented entropy measures to select significant sustainability indicators.
   - Adapted methods from literature for informative feature determination.

**Model Selection**
   - Evaluated classical and fuzzy clustering techniques for handling uncertain data categorization.
   - Utilized literature findings on fuzzy clustering effectiveness in sustainability assessments.

**Model Training**
   - Applied hierarchical agglomerative clustering with a fuzzy membership matrix.
   - Adapted standard hierarchical methods to include fuzzy logic for nuanced state grouping.

**Model Evaluation**
   - Compared clustering outputs using centroid link, single link, and complete link metrics.
   - Assessed classical versus fuzzy-enhanced hierarchical methods for capturing state similarities.

**Model Tuning**
   - Iteratively refined fuzzy clustering parameters and weighting schemes.
   - Focused on entropy-based weighting adjustment for model sensitivity to relevant features.

**Deployment**
   - Presented results in academic and policy-making venues.
   - Shared findings through conferences, publications, and engagements with policymakers.

## Models Overview

### Hierarchical Agglomerative Clustering (HAC)
- Begins with each state as its own cluster and merges them based on the closest distance metrics until all are unified into a single cluster.
  - Enhanced with fuzzy logic to manage the overlapping nature of sustainability metrics across states

### Fuzzy Membership Matrix Based Clustering
- Utilizes a membership matrix to determine the degree of belonging each state has to each cluster, updating iteratively based on state similarities.
  - Addresses the issue of states having multiple sustainability profiles by enabling partial membership across clusters, a significant deviation from traditional hard clustering methods.

### Naive Weighted Fuzzy Membership Matrix
- Applies a naive weighting system based on standard deviations and means of sustainability indicators to adjust the influence of each feature within the clustering process.
  - Introduces a simple yet effective form of feature weighting to enhance the membership matrix, making the model sensitive to the most impactful sustainability features.

### Entropy Weight Based Fuzzy Membership Matrix
- Implements the entropy weight method to calculate the dispersion of data, which helps in quantifying how much information each attribute contributes to the overall clustering.
  - This sophisticated weighting mechanism significantly refines cluster formations by prioritizing data points that offer the most distinctive insights into state sustainability.

In our paper, each model is evaluated against classical metrics such as centroid, single, and complete link to validate their effectiveness. 

The models are iteratively tuned based on these evaluations to enhance their precision and reliability in distinguishing between the sustainability profiles of different states.

We hope that integration of these models provides a comprehensive toolset for policymakers and researchers to categorize states in a way that reflects their true sustainability characteristics.

## Data
- [Energy Consumption by State since 1990](data/raw/annual_consumption_state.xls)
- [Energy Generation by State since 1990](data/raw/annual_generation_state.xls)
- [Carbon Emissions by State in Various Sectors](https://www.eia.gov/environment/emissions/state/)
- Additional data from EPA, US Census Bureau, and CDC.


## Authors
<table>
  <tr>
    <td>

**Prayash Joshi**  
Lead ML Engineer/Researcher  
[LinkedIn](https://www.linkedin.com/in/prayashjoshi/) | [Github](https://github.com/prayashjoshi)

</td>
    <td>

**Arsh Siddiqui**  
Lead Data Scientist/Researcher  
[Github](https://github.com/ArshSiddiqui)

</td>
    <td>

**Charles Brune**  
Lead Data Engineer/Developer  

</td>
  </tr>
</table>
