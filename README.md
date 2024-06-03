# Weather_Prediction_HMM
This project analyzes Seattle weather data and uses a Hidden Markov Model (HMM) to predict the weather based on various encoded features such as season, temperature, precipitation, and wind.

## Features

- Data preprocessing and feature encoding
- Basic data exploration and visualization
- Implementation of Gaussian HMM for weather prediction
- Evaluation of model performance using different parameter combinations

## Getting Started

### Prerequisites

- Python 3.6 or later
- Required Python libraries: `pandas`, `numpy`, `hmmlearn`, `matplotlib`, `seaborn`, `tqdm`


### Running the Analysis

1. Place the `seattle-weather.csv` file in the `sample_data` directory.

2. Run

### Data

The dataset used for this analysis is `seattle-weather.csv`, which contains the following columns:

- `date`: The date of the observation
- `precipitation`: The amount of precipitation (in inches)
- `temp_max`: The maximum temperature (in degrees Celsius)
- `temp_min`: The minimum temperature (in degrees Celsius)
- `wind`: The average wind speed (in meters per second)
- `weather`: The weather condition (e.g., drizzle, rain, sun, etc.)

### Code Overview

- `weather_analysis.py`: The main script that performs data preprocessing, feature encoding, model training, and evaluation.
- `sample_data/seattle-weather.csv`: The dataset used for analysis.

### Feature Encoding

The following features are encoded for use in the HMM model:

- `Encode Weather`: Encoded values for weather conditions
- `Encode Season`: Encoded values for seasons (0: winter, 1: spring, 2: summer, 3: autumn)
- `Encode Temp`: Encoded values for temperature ranges (0: very cold, 1: cold, 2: cool, 3: warm)
- `Encode Precipitation`: Binary encoding for precipitation (0: none, 1: precipitation)
- `Encode Wind`: Encoded values for wind speed ranges

### Model Evaluation

The model is evaluated using different combinations of the number of components in the HMM and the number of previous days considered. The performance is visualized using heatmaps and plots.

### Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes
