# public-api-json-parsing

Python notebooks that pull data from public U.S. government APIs and load the
JSON responses into pandas DataFrames. I wrote them in Databricks as my part of
an internal Databricks hackathon, hoping to use this data in our build. They
weren't part of the final project, so this repo stands on its own. (The
hackathon project itself is not public.)

| Notebook | Source | Data |
|---|---|---|
| `ACS_api.ipynb` | U.S. Census Bureau, American Community Survey | Demographic and housing data |
| `BEA_api.ipynb` | Bureau of Economic Analysis | Regional and national economic accounts |
| `BLS_api.ipynb` | Bureau of Labor Statistics | Employment, wage and price data |
| `FRED_api.ipynb` | Federal Reserve Bank of St. Louis (FRED) | Federal funds rate and target range limits |
| `HUD_api.ipynb` | Dept. of Housing and Urban Development | Housing data |

## Approach
- Calls each API with `requests` (with timeouts) and loads the JSON into pandas
- API keys are read from Databricks secrets, not stored in the code

