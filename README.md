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
6. `model_num_trips_nn.ipynb` followed by `model_avg_pay_nn`: These notebooks train and test a neural network to predict the number of trips and average driver pay in any given hour, outputting predictions and true values of the test set
7. `model_num_trips_rf.ipynb` followed by `model_avg_pay_rf`: These notebooks train and test a random forest classifier to predict the number of trips and average driver pay in any given hour, outputting predictions and true values of the test set
8. `model_analysis.ipynb`: This notebook is used to create visualisations comparing performance of the models