# data-512-project

I'm studying how wildfires affect Yakima, Washingtonn. I gathered wildfire and air quality data, made a guess of how much smoke might affect the city, and compared it to the actual air quality numbers. I also looked at how often wildfires happen, how much area they burn, and used this information to guess the smoke levels for the next 25 years.

## Source Data
Combined wildland fire datasets for the United States and certain territories, 1800s-Present (combined wildland fire polygons) https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81

Wildfire Cities Assignment https://docs.google.com/spreadsheets/d/1cmTW5fgU3KyH6JbrRao-qWjzu2GovKk_BkA7a-poGFw/edit#gid=1247370552

# Coding Process
In my project, I first tackle a large 2.8GB dataset from USGS about wildfires, focusing on events since 1963 near Yakima, WA, and creating a detailed smoke impact assessment. This part of the work produces a big file, smoke_estimate_yakima.json, which is too large for Github.

Next, I acquire Air Quality Index (AQI) data by using an EPA API key to fetch historical air quality records. Since Yakima lacks local weather stations, I have to cast a wider net, searching up to 250 miles away to find relevant data. This effort results in a comprehensive aqi.csv file covering the years 1985-2022.

Lastly, I analyze the wildfire data and AQI, visualizing the findings and predicting future smoke levels with a forecast extending 25 years, thanks to the Prophet forecasting tool. All these steps are detailed in a separate Reflections document.


