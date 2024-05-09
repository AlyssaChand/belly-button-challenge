# belly-button-challenge
These are the sources I used to help write my code: [https://developer.mozilla.org/](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference), google, and BCS — watching our cloud recordings, using instructor activity solutions and the class activities as references.

In this assignment, the task is to build an interactive dashboard to explore the [Belly Button Biodiversity dataset](http://robdunnlab.com/projects/belly-button-biodiversity/), which catalogs the microbes that colonize human navels.

![Screenshot 2024-05-09 130029](https://github.com/AlyssaChand/belly-button-challenge/assets/151655013/8250bc94-9544-4fd4-be7b-48e6d5ef8df5)

Here are the steps I did to achieve this:

### Building Metadata Panel

1. Retrieve metadata from the JSON file.
2. Filter the metadata for the desired sample.
3. Select the HTML panel where the metadata will be displayed.
4. Clear any existing metadata in the panel.
5. Append new HTML tags for each key-value pair in the filtered metadata, displaying them in uppercase format.

### Building Charts

1. Retrieve sample data from the JSON file.
2. Filter the sample data for the desired sample.
3. Extract `otu_ids`, `otu_labels`, and `sample_values` from the filtered sample object.
4. Build a Bubble Chart using the extracted data.
5. Define the layout for the Bubble Chart.
6. Render the Bubble Chart.
7. Prepare data for a Bar Chart by selecting the top 10 bacteria cultures found.
8. Build a Bar Chart using the prepared data.
9. Define the layout for the Bar Chart.
10. Render the Bar Chart.

### Run on Page Load

1. Retrieve sample names data from the JSON file.
2. Select the dropdown element where sample names will be displayed.
3. Populate the dropdown options with sample names.
4. Get the name of the first sample from the list.
5. Build charts and metadata panel with the data of the first sample.

### Event Listener and Dashboard Initialization

1. Update charts and metadata by calling buildCharts(newSample) and buildMetadata(newSample) functions.
2. The init() function is called to initialize the dashboard when the webpage loads.

### CSS Styling

To achieve consistency with the image for Demographic Info provided in the module instructions, I added css styling in the HTML file.

1. .card-primary: This selector sets the border color of the card containing demographic information to a shade of steel blue.
2. .card-primary .card-header: This selector sets the background color of the card header to steel blue and the text color to white.



