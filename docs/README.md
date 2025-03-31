# OHLC_gold_timeseries

This project builds an interactive OHLC (Open-High-Low-Close) chart using Plotly and D3.js. The chart visualizes historical gold price data (in USD), loading it from a CSV file.

Libraries Used:
- Plotly (https://plot.ly) for interactive charting
- D3.js (https://d3js.org/) for CSV file parsing

Data Source: Gold USD Historical Prices from Kaggle (https://www.kaggle.com/datasets/mesutssmn/gold-usd-price-dataset/data)

File Structure:
- index.html : Contains the HTML, JavaScript, and configuration for rendering the OHLC chart.
- data/gold_usd_price.csv: The CSV file with historical gold price data.


Setup and Usage
- Clone or Download the Repository: Download the project files to your local machine.
- Run a Local Web Server: Because the CSV file is loaded via JavaScript, running the project on a local web server helps avoid CORS issues. For example, if you have Python installed, navigate to the project directory and run:
    python -m http.server 8000
  
- Open your browser and go to:
    http://localhost:8000

- View the Chart: Open index.html in your browser via the local server. The OHLC chart should render automatically.
    http://localhost:8000/ohlc.html

Credits Data Source: Kaggle - Gold USD Historical Prices (https://www.kaggle.com/datasets/mesutssmn/gold-usd-price-dataset/data)

License: This project is licensed under the MIT License. 
