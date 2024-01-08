# Mars Data Scraping and Analysis

## Part 1: Scrape Titles and Preview Text from Mars News

### Instructions
1. Open the Jupyter Notebook `part_1_mars_news.ipynb` in the starter code folder.
2. Utilize automated browsing to visit the Mars News website.
3. Inspect the page to identify the elements to scrape.
   - **Hint:** Create a Beautiful Soup object to extract text elements from the website.
4. Extract titles and preview text of the news articles.
   - Store each title-and-preview pair in a Python dictionary with keys 'title' and 'preview'.
     - Example:
     ```python
     {'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm", 
      'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}
     ```
   - Store all dictionaries in a Python list.
5. Print the list in your notebook.
6. Optionally, store the scraped data in a file (e.g., JSON).

## Part 2: Scrape and Analyze Mars Weather Data

### Instructions
1. Open the Jupyter Notebook `part_2_mars_weather.ipynb` in the starter code folder.
2. Use automated browsing to visit the Mars Temperature Data Site.
3. Inspect the page to identify the elements to scrape (URL: https://static.bc-edx.com/data/web/mars_facts/temperature.html).
   - **Hint:** Create a Beautiful Soup object to scrape data from the HTML table.
4. Assemble the scraped data into a Pandas DataFrame with columns matching the table on the website.
   - Columns: id, terrestrial_date, sol, ls, month, min_temp, pressure.
5. Analyze the dataset using Pandas functions to answer the following questions:
   - How many months exist on Mars?
   - How many Martian (not Earth) days of data are in the dataset?
   - What are the coldest and warmest months on Mars?
     - Find average minimum daily temperature for all months and plot the results as a bar chart.
   - Which months have the lowest and highest atmospheric pressure on Mars?
     - Find average daily atmospheric pressure for all months and plot the results as a bar chart.
   - Estimate the number of terrestrial days in a Martian year.
     - Consider Earth days elapsed in the time Mars circles the Sun.
     - Visually estimate the result by plotting the daily minimum temperature.
6. Export the DataFrame to a CSV file.
