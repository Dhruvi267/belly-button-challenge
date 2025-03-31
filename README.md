# Belly Button Biodiversity Dashboard

An interactive web dashboard to explore the [Belly Button Biodiversity Dataset](http://robdunnlab.com/projects/belly-button-biodiversity/).


## Features
- **Interactive Visualization**: 
  - Dropdown menu to select sample subjects
  - Dynamic updates of all visualizations when selection changes
- **Charts**:
  - Horizontal bar chart showing top 10 microbial species (OTUs)
  - Bubble chart displaying all microbial species in sample
- **Demographic Info Panel**: Displays metadata for selected test subject

## Technologies Used
- **JavaScript** (D3.js for data manipulation, Plotly.js for visualization)
- HTML/CSS
- Bootstrap framework

## Usage
1. Select test subject ID from dropdown menu
2. View demographic information in metadata panel
3. Explore microbial composition through interactive charts:
   - Hover over chart elements for additional details
   - Bar chart shows top 10 most abundant microbial species
   - Bubble chart shows relative frequency of all species

## Data Source
Dataset obtained from:  
[Rob Dunn Lab](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)  
Contains:
- 1536 samples
- Microbial species (OTU) data
- Demographic information for test subjects

## Code Structure
```bash
belly-button-challenge/
├── index.html         # Main application page
├── samples.json       # Sample dataset (reference)
└── static/
    ├── css/           # CSS styles
    └── js/
        └── app.js     # Main application logic
```

## Key Code Implementation
### Data Fetching & Initialization
```javascript
d3.json(url).then(function(data) {
    // Initialize dropdown and charts
});
```

### Dynamic Chart Updates
```javascript
function buildCharts(sampleID) {
    // Bar chart and bubble chart configuration
}

function buildMetadata(sampleID) {
    // Metadata panel updates
}
```
