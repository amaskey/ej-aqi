### Environmental justice means the fair treatment of all people from environmental impacts, regardless of race, color, national origin, education level, or income. This code uses machine learning (ML) to model air quality disparities in Jefferson County, Alabama.

### Source code:
- cnn-lstm-daily.ipynb is a Google Colab Notebook that implements the CNN-LSTM approach to train a model to predict AQI based on historical data and correlates with demographic information.
- predicting-AQI-population-projection.ipynb is a Google Colab Notebook that uses the trained model to predict AQI values for projected population for future years.

### Data:
The two curated datasets are daily-data-ml-ready.csv and population-projection-ml-ready.csv. 
- The daily-data-ml-ready.csv file includes daily AQI for seven distinct locations in Jefferson County for the past nine years. It also incudes the computed AQI with relation to race demographics.
- The population-projection-ml-ready.csv file includes annual aggregation of AQI and projected population for race demographics.

### Visualization:
The visualization folder contains six images. 
- aqi-onmap.png shows 7 different locations in Jefferson County with AQI sensors. Color range corresponds to the AQI level.
- aqi-sensor.JPG is an image of an air quality sensor that I am building.
- aqi-timeseries-jeffersoncounty.png shows a summary view of air quality and socio-economic information for Jefferson County. It includes major air quality sensor locations and the days with AQI over 100 (unhealthy), a satellite view of ZIP codes 35207 and 35094, highlighting demographics information, and annual AQI time series for years 2015, 2019, and 2023, comparing ZIP codes 35207 and 35094.
- predictted-AQI-population-projection.png shows how AQI changed for population projections of the entire county, as well as for specific marginalized communities.
- target-vs-prediction-aqi.png shows how my model performed in predicting AQI values for test data by plotting the true value for AQI and the predicted AQI value.
- training_curve.png shows the training loss and validation loss of CNN-LSTM model, both of which stabilize as the number of epochs increases.
