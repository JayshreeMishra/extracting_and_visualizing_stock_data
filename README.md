# Extracting and Visualizing Stock Data

## Overview

This project involves extracting and visualizing stock data for two companies, Tesla and GameStop. The data is obtained using the `yfinance` library to fetch historical stock prices and web scraping to extract revenue data. The extracted data is then visualized using `plotly` to create interactive and informative graphs.

## Code Structure

### Libraries Used
- `yfinance`: Used to extract historical stock data.
- `pandas`: Used for data manipulation and analysis.
- `requests`: Used for making HTTP requests to scrape web data.
- `BeautifulSoup`: Used for web scraping to parse HTML content.
- `plotly`: Used for creating interactive and visually appealing plots.

### Functions

#### `make_graph(stock_data, revenue_data, stock)`

This function takes three parameters (`stock_data`, `revenue_data`, and `stock`) and creates a subplot with historical share price and historical revenue using `plotly`. The steps include:
1. Creating a subplot with two rows for historical share price and historical revenue.
2. Filtering the data based on specific dates.
3. Adding traces for historical share price and historical revenue to the respective subplots.
4. Updating the layout of the graph, including axis titles and overall layout settings.
5. Displaying the graph.

### Data Extraction

#### Tesla Stock Data
- Using `yfinance` to fetch historical stock data for Tesla (`TSLA`).
- Extracting relevant columns such as Date, Open, High, Low, Close, Volume, Dividends, and Stock Splits.

#### Tesla Revenue Data
- Web scraping Tesla's annual revenue data from a specified URL.
- Cleaning and formatting the data for analysis.

#### GameStop Stock Data
- Using `yfinance` to fetch historical stock data for GameStop (`GME`).
- Extracting relevant columns similar to Tesla's stock data.

#### GameStop Revenue Data
- Web scraping GameStop's annual revenue data from a specified URL.
- Cleaning and formatting the data for analysis.

### Data Visualization

#### Tesla Stock Graph
- Plotting the historical share price and revenue of Tesla using the `make_graph` function.
- Utilizing interactive features of `plotly` for a better user experience.

#### GameStop Stock Graph
- Plotting the historical share price and revenue of GameStop using the `make_graph` function.
- Leveraging the interactive capabilities of `plotly` for a dynamic representation.

## Instructions

1. Install the required libraries by running `pip install yfinance pandas requests beautifulsoup4 plotly`.
2. Run the provided code sections to extract and visualize Tesla and GameStop stock data.
3. Explore the interactive graphs to gain insights into the historical trends of share prices and revenues for the respective companies.

## Note on Visualizations

The Jupyter Notebook in this repository includes interactive visualizations that may not be visible directly on GitHub. GitHub provides a static view of Jupyter Notebooks, which means the code executes but doesn't display dynamic content such as plots.

**Check Images Below:**

##### Tesla Stock Graph
![Tesla_stock_graph](https://github.com/JayshreeMishra/images/blob/main/tesla.png)

##### GameStop Stock Graph
![GameStop_Stock_Graph](https://github.com/JayshreeMishra/images/blob/main/gme.png)


Feel free to customize the code or contribute to enhance the functionality of this project. If you encounter any issues, please refer to the documentation of the used libraries or create an issue in the repository.
