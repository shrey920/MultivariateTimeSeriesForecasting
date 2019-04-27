# Multivariate Time Series Forecasting

This project is an implementation of the paper [Modeling Long- and Short-Term Temporal Patterns with Deep Neural Networks](https://arxiv.org/abs/1703.07015) .

## Requirements

This project uses python 3.6 and the PIP the packages included in requirements.txt 
### Use virtualenv
```
virtualenv -p python3 venv

source /venv/bin/activate

pip install -r requirements.txt

```
## Dataset
Create folder /data/ and store raw text format dataset in it.
The exchange dataset is already present in the data folder.
## For other datasets advisable to run on GPU or colab version:
### Electricity consumption


The raw dataset is in https://archive.ics.uci.edu/ml/datasets/ElectricityLoadDiagrams20112014. It is the electricity consumption in kWh was recorded every 15 minutes from 2011 to 2014. Because the some dimensions are equal to 0. So we eliminate the records in 2011. Final we get data contains electircity consumption of 321 clients from 2012 to 2014. And we converted the data to reflect hourly consumption.

### Traffic Usage

The raw data is in http://pems.dot.ca.gov. The data in this repo is a collection of 48 months (2015-2016) hourly data from the California Department of Transportation. The data describes the road occupancy rates (between 0 and 1) measured by different sensors on San Francisco Bay area freeways.

### Solar Energy

The raw data is in http://www.nrel.gov/grid/solar-power-data.html : It contains the solar power production records in the year of 2006, which is sampled every 10 minutes from 137 PV plants in Alabama State.  

## Running the Local Version

Run the LSTNet.ipynb file on jupyter notebook.

## Google Colab with GPU

The code needs a gpu environment for fast execution for datasets of elecrticity, solar and traffic.

Upload the the file MultivariateTimeSeriesForecasting(colab_version).ipynb on a new cuda10 enabled colab project.
Add this [link](https://drive.google.com/open?id=1OHtGDWiBhkeFqU6sar6Op7pyykkVhgUo) to your drive for retrieving the datasets.


