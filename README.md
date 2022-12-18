# Credit Union Planner Challenge
This is a Jupyter Notebook that uses API calls to analyse a hypothetical returns and portfolio analysis. This helps the user evaluate their financial health. The user can see how their crytocurrency potrfolio is as well as their stocks and bonds current value. Part two of the notebook the user can see their retirement health. Using an alpaca API call and a Monte Carlo simulation the user is able to see their reitrent possible outcomes with different weights assigned to different stocks or bonds. 
---

## Technologies

This project leverages python 3.7 with the following packages:

* [pandas](https://github.com/pandas-dev/pandas) - For the command line interface, help page, and entrypoint.

* [numpy](https://github.com/numpy/numpy) - for entry point, and help page.

* [dotenv](https://github.com/vlucas/phpdotenv) - reads .env files seperate from the environmnet 

* [alpaca-api-call](https://github.com/alpacahq/alpaca-trade-api-python)-python library for the Alpaca Commission Free Trading API. 

* [nasdaq-api-call](https://github.com/Nasdaq/NasdaqCloudDataService-REST-API)- method of delivery for realtime exchange data and other financial information

* [metaplot](https://github.com/matplotlib/matplotlib) - For entrypoint and help page.

---

## Installation Guide

Before running the application first install the following dependencies.

```python
import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation
%matplotlib inline
```


---

## Usage

Acitvate a Jupyter Lab Notebook by having the kernal installed and typing `jupyter lab` in your terminal. 

User mush have the 'MCForcastTools.py' moduel in order to run the simulation.

---

## Examples

```
alpaca = tradeapi.REST(
    alpaca_api_key,
    alpaca_secret_key,
    api_version = "v2")

tickers = ["SPY","AGG"]

timeframe = "1D"

start_date = pd.Timestamp("2022-12-14", tz="America/New_York").isoformat()
end_date = pd.Timestamp("2022-12-14", tz="America/New_York").isoformat()
```

---

## Contributors

DU Starter Code
Terrence McCoy

MCForcastTools.py

Alpaca 
NADSAQ

---

## License

MIT
