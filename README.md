# data_week14

Belly Button Biodiversity Dashboard
Overview
This project visualizes microbial biodiversity in human belly buttons using an interactive dashboard. The dataset is based on a study that analyzed bacteria found in various individuals' navels. The dashboard allows users to explore the data through dynamic charts and metadata panels.

Files Included
1. index.html
The main HTML file that serves as the dashboard.
Loads external libraries including:
D3.js (d3.v7.min.js) for data handling.
Plotly (plotly-latest.min.js) for data visualization.
Bootstrap (bootstrap.min.css) for styling.
Contains a dropdown for selecting a test subject and sections for displaying metadata and visualizations.
2. samples.json
The dataset containing information about microbial samples.

Main Components:
names: List of test subject IDs.
metadata: Demographic information for each test subject (e.g., age, location, and wash frequency).
samples: Bacterial data for each subject, including:
otu_ids: Identifiers for bacterial species.
sample_values: Quantities of each bacterial species.
otu_labels: Taxonomic classifications.
4. app.js
JavaScript file responsible for data retrieval and visualization.

Functions:
init(): Initializes the dashboard with the first test subject's data.
optionChanged(newSample): Updates the charts and metadata panel when a new subject is selected.
buildMetadata(sample): Displays demographic information of the selected subject.
buildCharts(sample): Creates:
Bar Chart: Top 10 most common bacteria in a sample.
Bubble Chart: Distribution of all bacterial species.
Usage
Open index.html in a browser.
Select a test subject from the dropdown.
View their metadata and bacterial composition in the interactive charts.
Data Source
The data originates from the Belly Button Biodiversity study by the Rob Dunn Lab.
More details: Belly Button Biodiversity Study.
Dependencies
D3.js
Plotly.js
Bootstrap
