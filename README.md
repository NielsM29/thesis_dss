<h1>Improving interpretability for forecasting of empirical nonlinear time-series using the SINDy algorithm</h1>

<h2>Purpose</h2>
This github repository has been created to supplement the thesis written in partial fulfillment of the requirements for the degree of master of science in Data Science & Society at the School of Humanities and Digital Sciences of Tilburg University. 

<h2>Files</h2>
This repository contains multiple files for the analysis provided in the thesis. Their uses are the following:

<h3>cloudiness.txt</h3>
Contains the time-series for the 'cloudiness' feature and the quality of the feature. Quality is used to indicate missing or impossible values.

Klein Tank, A.M.G. and Coauthors, 2002. Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. Int. J. of Climatol., 22, 1441-1453. Data and metadata available at http://www.ecad.eu

<h3>humidity.txt</h3>
Contains the time-series for the 'humidity' feature and the quality of the feature. Quality is used to indicate missing or impossible values.

Klein Tank, A.M.G. and Coauthors, 2002. Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. Int. J. of Climatol., 22, 1441-1453. Data and metadata available at http://www.ecad.eu

<h3>max_temp.txt</h3>
Contains the time-series for the 'max_temp' feature and the quality of the feature. Quality is used to indicate missing or impossible values.

Klein Tank, A.M.G. and Coauthors, 2002. Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. Int. J. of Climatol., 22, 1441-1453. Data and metadata available at http://www.ecad.eu

<h3>mean_temp.txt</h3>
Contains the time-series for the 'mean_temp' feature and the quality of the feature. Quality is used to indicate missing or impossible values.

Klein Tank, A.M.G. and Coauthors, 2002. Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. Int. J. of Climatol., 22, 1441-1453. Data and metadata available at http://www.ecad.eu

<h3>min_temp.txt</h3>
Contains the time-series for the 'min_temp' feature and the quality of the feature. Quality is used to indicate missing or impossible values.

Klein Tank, A.M.G. and Coauthors, 2002. Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. Int. J. of Climatol., 22, 1441-1453. Data and metadata available at http://www.ecad.eu

<h3>precipitation.txt</h3>
Contains the time-series for the 'precipitation' target feature and the quality of the target feature. Quality is used to indicate missing or impossible values.

Klein Tank, A.M.G. and Coauthors, 2002. Daily dataset of 20th-century surface air temperature and precipitation series for the European Climate Assessment. Int. J. of Climatol., 22, 1441-1453. Data and metadata available at http://www.ecad.eu

<h3>preprocessing & EDA.ipynb</h3>
Contains code writen for the creation of the dataset used, as well as the pre-processing and exploratory data analysis performed for the thesis. In order to run this code, the .txt files for the following features need to be available: cloudiness, humidity, max_temp, mean_temp, min_temp & precipitation.

Running this file creates two folders.

The 'dataset' folder contains three datasets:
1. The unprocessed dataset
2. The processed raw dataset
3. The processed denoised dataset

The 'graph' folder contains several graphs, among which:
1. Time-series of features before pre-procesisng
2. Time-sereis of features after pre-processing
3. Autocorrelation plots

<h3>SINDy_number(raw/denoised).ipynb</h3>
Files used for validation of SINDy algorithm and generating results on test set. In order to run these files, the datasets extracted through the preprocessing & EDA.ipynb file are necessary for running this file.

#1 indicates the SINDy implementations incl. lagged features
#2 indicates the SINDy implementations excl. lagged features

(raw) indicates the analysis performed on the raw dataset
(denoised) indicates the analysis performed on the denoised dataset

Running these files generate results for the SINDy algorithm.

<h3>LSTM(raw/denoised).ipynb</h3>
Files used for validation of the LSTM algorithm and generating results on test set. In order to run these files, the datasets extracted through the preprocessing & EDA.ipynb file are necessary for running this file.

(raw) indicates the analysis performed on the raw dataset
(denoised) indicates the analysis performed on the denoised dataset

Running these files generate results for the LSTM algorithm and add loss plots to the 'graphs' folder

<h3>graphs_creation_results.ipynb</h3>
File used for generating plots to compare SINDy and LSTM performance. In order to run this file, the datasets extracted through the preprocessing & EDA.ipynb file are necessary for running this file.

Running this file generates plots to compare the performance of SINDy to LSTM and ads them to the 'graphs' folder
