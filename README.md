# Belly Button Biodiversity Dashboard

## Preview

This application is an interactive dashboard to analyze the relative abundance of different microbial “species” (technically operational taxonomic units, OTUs) across large taxonomic data matrix and meta-data matrix for [belly buttons microbes samples](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/).
It's a useful tool for investigating the microbes inhabiting our navels and the factors that might influence the microscopic life.

[View Website](https://belly-button-biodiversity73.herokuapp.com/)

## Method & Usage

### Step 1 - Flask API

  * Use Flask to design an API for loading dataset and to serve the HTML and JavaScript required for dashboard page 
  
  * Use the Bootstrap grid system to create the structure of the dashboard page

### Step 2 - Use Plotly.js to build interactive charts for the dashboard

  * Use the route /names to populate a dropdown select element with the list of sample names
  
  * Create a function called optionChanged to handle the change event when a new sample is selected (i.e. fetch data for the newly selected sample)
  
  * Create a PIE chart that uses data from samples route to display the top 10 samples

  * Create a Bubble Chart that uses data from samples route to display each sample

  * Display each key/value pair from the metadata JSON object on the page

  * Update all of the plots any time that a new sample is selected
  
  * Adapt the Gauge Chart to plot the Weekly Washing Frequency

### Step 3 - Deploy Flask app to Heroku

  * Use sqlite database to load and save new data

