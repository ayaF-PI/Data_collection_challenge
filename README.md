# Data_collection_challenge

# Mars Weather Data Analysis


# Overview
This project involves scraping, cleaning, analyzing, and visualizing data related to Mars' weather conditions, such as minimum temperature and atmospheric pressure. The data is collected from a Mars temperature data website using web scraping techniques and is further processed for analysis using Pandas. The project provides insights into the seasonal temperature and pressure variations on Mars and estimates the length of a Martian year.

# Deliverables
Deliverable 1: Scrape Titles and Preview Text from Mars News
The first part of the project involved scraping titles and preview text from the Mars News website using Splinter and BeautifulSoup. The extracted data is stored in a Python list of dictionaries and is further saved to a JSON file.

Deliverable 2: Scrape and Analyze Mars Weather Data
The second part of the project involves scraping weather data (such as minimum temperature and pressure) from the Mars Temperature Data website, processing it into a Pandas DataFrame, and performing analysis on the dataset to answer key questions.

# Project Structure
part_1_mars_news.ipynb: Jupyter Notebook for scraping and storing Mars news articles' titles and preview texts.
part_2_mars_weather.ipynb: Jupyter Notebook for scraping Mars weather data, cleaning the data, analyzing it, and visualizing the results.
mars_weather_data.csv: Exported CSV file containing the cleaned and processed Mars weather data.
README.md: This README file explaining the project structure and its contents


# Steps and Analysis
1. Scrape Titles and Preview Text from Mars News
Using Splinter and BeautifulSoup, titles and preview texts from the Mars News website were scraped. Each news article's title and preview text were stored in a list of dictionaries, which was further exported as a JSON file.

2. Scrape and Analyze Mars Weather Data
a. Scrape Mars Weather Data
The Mars Temperature Data website was visited using Splinter. The table containing weather data was scraped using BeautifulSoup and stored in a Pandas DataFrame for further analysis.

b. Clean and Process the Data
The data was cleaned and the appropriate data types (e.g., datetime, float, and int) were assigned to the respective columns. The columns included:

id: Identification number for each record.
terrestrial_date: Earth date.
sol: Martian day count.
ls: Solar longitude.
month: Martian month.
min_temp: Minimum temperature (°C) on Mars.
pressure: Atmospheric pressure (Pa) on Mars.
c. Data Analysis
The dataset was analyzed to answer the following questions:

How many unique months exist on Mars?
How many Martian days (sols) worth of data exist in the dataset?
What are the coldest and warmest months on Mars (based on average minimum temperature)?
Which months have the lowest and highest atmospheric pressure?
How many Earth days exist in a Martian year (estimated by analyzing temperature cycles)?
d. Visualizations
Average Minimum Temperature by Month: A bar chart visualizing the coldest and warmest months based on temperature.
Average Atmospheric Pressure by Month: A bar chart visualizing the months with the lowest and highest pressure.
Daily Minimum Temperature over Time: A line plot showing the cyclic nature of Martian temperature, helping to estimate the length of a Martian year.
3. Save the Data
The processed and cleaned data was exported to a CSV file (mars_weather_data.csv) for further use and sharing.

# Results
Minimum Temperature:

The coldest month is Month 3 with an average minimum temperature of around -83°C.
The warmest month is Month 8 with an average minimum temperature of -68°C.
Atmospheric Pressure:

The lowest atmospheric pressure is observed in Month 6 (around 700 Pa).
The highest atmospheric pressure occurs in Month 9 (around 925 Pa).
Year Length:

By analyzing the temperature cycles, we estimate that a Martian year lasts approximately 687 Earth days.


# Conclusion
This project provides valuable insights into the climate conditions on Mars, focusing on temperature and pressure variations and the length of a Martian year. The use of web scraping, data cleaning, and analysis techniques demonstrates how Python can be used for scientific data analysis in space exploration contexts.
