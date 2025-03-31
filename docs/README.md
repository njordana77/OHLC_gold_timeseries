# OHLC_gold_timeseries

This project builds an interactive OHLC (Open-High-Low-Close) chart using Plotly and D3.js. The chart visualizes historical gold price data (in USD), loading it from a CSV file.
Overview

Chart Type: OHLC (Open-High-Low-Close) Chart

Libraries Used:

    Plotly (https://plot.ly) for interactive charting

    D3.js (https://d3js.org/) for CSV file parsing

Data Source:

    Gold USD Historical Prices from Kaggle (https://www.kaggle.com/datasets/mesutssmn/gold-usd-price-dataset/data)

File Structure

index.html

    Contains the HTML, JavaScript, and configuration for rendering the OHLC chart.

data/gold_usd_price.csv

    The CSV file with historical gold price data.

    Ensure this file is in a folder named "data" relative to index.html.

Setup and Usage

    Clone or Download the Repository:

        Download the project files to your local machine.

    Verify File Paths:

        Confirm that gold_usd_price.csv is located in a folder named "data" in the same directory as index.html.

    Run a Local Web Server:

        Because the CSV file is loaded via JavaScript, running the project on a local web server helps avoid CORS issues.

        For example, if you have Python installed, navigate to the project directory and run:

        python -m http.server 8000

        Open your browser and go to: http://localhost:8000

    View the Chart:

        Open index.html in your browser via the local server.

        The OHLC chart should render automatically.

        If you encounter issues, check the browser console for errors related to file loading or script issues.

Customization

    CSV File Path:

        The code loads the CSV using: d3.csv("data/gold_usd_price.csv")

        Modify this path if your CSV file is stored elsewhere.

    Time Settings:

        Each date is adjusted by setting the time with: dt.setHours(12, 0, 0, 0);

        Change this if you need to display a different time (e.g., 9:30 AM ET).

    Chart Appearance:

        Customize the chart’s layout, colors, and interactivity within the JavaScript section in index.html.

Troubleshooting

    CSV Loading Issues:

        If the chart does not render, verify that the CSV file is accessible.

        Open the browser’s developer console (usually via F12) to check for error messages.

    Local Server:

        Opening the HTML file directly with the file:// protocol may cause CORS errors.

        Running a local web server is recommended.

Credits

    Plotly: https://plot.ly

    D3.js: https://d3js.org

    Data Source: Kaggle - Gold USD Historical Prices (https://www.kaggle.com/datasets/mesutssmn/gold-usd-price-dataset/data)

License
This project is licensed under the MIT License. 
