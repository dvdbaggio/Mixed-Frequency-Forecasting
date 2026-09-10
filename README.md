
# Mixed-Frequency Forecasting
Forecasting key accounting variables of Italian listed companies (MIB, Mid Cap and Small Cap) with LSTM-based sequence models, compared against xLSTM and econometric baselines.
  
## Overview
-  **Targets:** annual EBITDA, Net Income and ROA, expressed as size-normalized delta-ratio targets
-  **Inputs:** a mixed-frequency panel of daily market and macroeconomic series, monthly macro indicators and static firm features (prior-year fundamentals, ratios, sector and size encodings).
-  **Models:** shallow and stacked LSTM, multi-frequency LSTM, feature-grouped LSTM, xLSTM, AR and MIDAS baselines.

## Data
The dataset is not included in this repository as it combines licensed third-party market and company-fundamental data that cannot be redistributed, so `Dataset/` contains only preprocessing code.

## Setup
```bash
python -m venv .venv

source .venv/bin/activate

pip install -r requirements.txt
```
