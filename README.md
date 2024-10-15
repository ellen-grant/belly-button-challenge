#  Belly Button Biodiversity Dashboard

![dashboard](https://github.com/user-attachments/assets/b120a6b8-ff68-4e77-9b02-35a4db91dd1a)

## Overview
This project presents an interactive dashboard that visualizes the bacterial diversity found in human belly buttons. The dataset includes information about various Operational Taxonomic Units (OTUs) identified through DNA sequencing from samples collected from different individuals. The dashboard allows users to explore the top 10 bacterial species (OTUs) found in a sample and visualize the bacterial cultures per sample using a bubble chart.

Dataset:
Belly Button Biodiversity dataset
http://robdunnlab.com/projects/belly-button-biodiversity/

This dashboard provides:
1. A dropdown menu to select an individual's sample ID.
2. A **horizontal bar chart** that displays the top 10 bacterial OTUs found in the selected individual.
3. A **bubble chart** that visualizes the entire bacterial diversity for the individual.
4. A **metadata panel** displaying the individual's demographic information (e.g., age, gender, ethnicity, etc.).

## Features
- **Interactive Dropdown Menu**: Users can select a sample ID to dynamically update the visualizations and demographic information.
- **Bar Chart**: Displays the top 10 OTUs found in the selected individual.
- **Bubble Chart**: Visualizes the entire bacterial diversity across all OTUs for a selected individual, with marker size representing bacterial abundance.
- **Metadata Panel**: Displays relevant demographic data for each selected individual.

## Setup Instructions

### Requirements
Ensure you have the following software:
- A modern web browser (e.g., Chrome)
- A code editor (optional, e.g., Visual Studio Code)
- A local server (e.g., GitHub Pages or Python's `http.server` module for local testing)

### Files
- `index.html`: Contains the structure of the web page and links to required libraries (e.g., D3.js, Plotly).
- `app.js`: Contains the logic to load data, build charts, and populate metadata dynamically.
- `samples.json`: The dataset containing sample IDs, bacterial OTUs, and demographic information.

### Instructions
1. Clone this repository to your local machine.
    ```bash
    git clone https://github.com/your-username/belly-button-biodiversity-dashboard.git
    ```
2. Open the `index.html` file in a web browser, or run a local server to view the dashboard:
    - **Python Local Server**: If you have Python installed, you can run the following commands in the terminal:
      ```bash
      python -m http.server
      ```
      Then, open your browser and navigate to `http://localhost:8000/`.

3. If you wish to deploy the app, use a static page hosting service like **GitHub Pages**:
    - Commit all changes and push to your GitHub repository.
    - Enable GitHub Pages from the repository settings and set the source to the main branch.

## Limitations

1. **Dataset Size**: The dataset used here is relatively small and specific to belly button bacterial diversity. It does not cover a broader range of microbiomes across different body sites or other types of samples.
   
2. **Static Data**: The dashboard currently operates on a static dataset (`samples.json`). As new samples or data updates become available, the dataset would need to be manually updated. A live, dynamic connection to the dataset would enhance the app’s scalability.

3. **Limited Demographic Information**: The demographic data presented is minimal (age, gender, location, etc.). Additional data such as diet, lifestyle, or health conditions could provide more context and lead to more meaningful analyses.

4. **Mobile Responsiveness**: While the dashboard is built using Bootstrap and should adapt to different screen sizes, certain aspects of the visualization may not render optimally on smaller screens. The bubble chart, in particular, may be difficult to interpret on mobile devices.

## Potential Meaningful Analysis

1. **Correlation Between Demographics and Bacterial Diversity**: By analyzing the distribution of bacterial species across different individuals, we could explore correlations between demographic factors (age, gender, location) and microbiome diversity. For example, are there significant differences in bacterial diversity between age groups or geographical regions?

2. **Frequency of Specific Bacteria Across Individuals**: Analyzing which bacterial species are common across multiple samples could provide insights into the "core" human microbiome. Understanding the common bacteria found in belly buttons across various individuals might help researchers identify which species are more or less universal in human microbiomes.

3. **Microbiome and Hygiene Habits**: If data on individuals' hygiene habits were available, one could explore potential relationships between bacterial diversity and factors like shower frequency or use of antibacterial products. For instance, does more frequent washing reduce the diversity of the microbiome, or do certain species thrive despite regular hygiene practices?

4. **Outliers and Rare Bacteria**: Identifying outliers in the dataset — individuals with particularly high or low bacterial diversity — could offer clues about environmental or health-related factors influencing microbial communities. Rare bacteria found in only a few individuals might be linked to unique environmental exposures or health conditions.

5. **Bacterial Functions and Health Implications**: Although this dashboard focuses on bacterial taxonomy, future analysis could explore the functions of specific bacteria in the microbiome. Understanding whether these bacteria contribute to health or disease could have implications for future research into gut health, immune function, and more.


## References
Hulcr, J. et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. Retrieved from: http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/.
