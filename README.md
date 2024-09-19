# Belly Button Biodiversity Dashboard

## Background
This project aims to build an interactive dashboard to explore the [Belly Button Biodiversity dataset](http://robdunnlab.com/projects/belly-button-biodiversity/), which catalogs the microbes that colonize human navels. The dataset shows that a small number of microbial species (known as operational taxonomic units, or OTUs) are present in more than 70% of people, while the rest are relatively rare.

## Project Overview
In this project, an interactive dashboard is created using JavaScript and Plotly to visualize data from the Belly Button Biodiversity dataset. The project includes a horizontal bar chart, a bubble chart, and a panel displaying demographic information. The dashboard updates dynamically based on the selected sample.

## Key Features
1. **Horizontal Bar Chart**: Displays the top 10 OTUs found in the selected individual's sample.
    - The OTUs are labeled using `otu_ids`, with `sample_values` representing the values.
    - Hover text is provided using `otu_labels`.

2. **Bubble Chart**: Visualizes all OTUs in the sample.
    - `otu_ids` are used for the x-axis and `sample_values` for the y-axis.
    - Bubble sizes represent `sample_values`, and colors are mapped to `otu_ids`.
    - Hover text displays `otu_labels`.

3. **Demographic Information**: Displays metadata (demographic information) for each individual.
    - The demographic data is displayed in the `#sample-metadata` panel.
    - A loop is used to append key-value pairs to the panel.

4. **Dynamic Updates**: The plots update dynamically when a new sample is selected from the dropdown menu.

## Dataset
The dataset used in this project can be accessed at the following URL: [Belly Button Biodiversity Dataset](https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json).

## Files
The following files are used in this project:
- `index.html`: The HTML structure for the dashboard.
- `samples.json`: The JSON file containing the dataset (loaded via D3.js).
- `static/js/app.js`: The main JavaScript file for plotting and updating charts.
- Additional assets in the `static` folder.

## Instructions
To replicate or run this project, follow these steps:
1. Clone this repository: `git clone <yourrepository_url>`
2. Inside your local repository, copy the provided starter files (`index.html`, `samples.json`, `static` folder) into your project.
3. Use the D3 library to read the `samples.json` file from the provided URL.
4. Follow the instructions in the code to create:
    - A horizontal bar chart displaying the top 10 OTUs.
    - A bubble chart for the OTUs in the sample.
    - A demographic information panel.
5. Deploy the project to GitHub Pages.

## How to Run
1. Open the `index.html` file in a browser to view the interactive dashboard locally.

## Dependencies
- D3.js
- Plotly.js
- HTML/CSS

## Notes
- Be sure to check the browser console (`console.log`) during development to debug and visualize data at different stages.
- Regular commits are important to track progress and changes throughout the development process.

## Deployment
This project has been deployed using GitHub Pages. You can view it live [githubpage](https://elenaz93.github.io/belly-button-challenge/).

### App Successfully Deployed to GitHub Pages
The app is now fully functional and hosted on GitHub Pages. You can explore the interactive dashboard, view the top 10 OTUs, bubble charts, and demographic information dynamically by selecting a sample from the dropdown menu.

## Resources
- [Plotly.js Documentation](https://plotly.com/javascript/)
- Hulcr, J. et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. Retrieved from: http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/Links to an external site.
