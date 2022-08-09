# MAST30034 Project 1 README.md
- Name: Sen Turner
- Student ID: 1168692

**Research Goal:** My research goal is to analyse how driver's average fare and number of available trips changes based on certain conditions

**Timeline:** The timeline for the research area is February 2019 - January 2020.

To run the pipeline, please visit the `scripts` and `notebooks` directories and run the files in this order:
1. `weather_scraper.py`: This downloads the weather data into the `data/raw` directory. <- Script taken from https://github.com/Karlheinzniebuhr/the-weather-scraper
2. `preprocessing_notebook_part_1.ipynb`: This notebook downloads the raw High Volume FHV data and outputs it to the `data/raw` directory.
3. `preprocessing_notebook_part_2.ipynb`: This notebook details all the pre-processing and aggregating steps to produce one large dataset, including outlier detection and removal. Then outputs the dataset to the `data/curated` directory.
4. `data_analysis_average_fare.ipynb`: This notebook performs analysis on how average fare is impacted by pickup location, hour of the day, day of the week and weather
5. `data_analysis_trips.ipynb`: This notebook performs analysis on how number of trips is impacted by pickup location, hour of the day, day of the week and weather





3. `analysis.ipynb`: This notebook is used to conduct analysis on the curated data.
4. `model.py` and `model_analysis.ipynb`: The script is used to run the model from CLI and the notebook is used for analysing and discussing the model.
