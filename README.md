<a name="readme-top"></a>

# 📗 Table of Contents

- [📖 About the Project](#about-project)
  - [🛠 Built With](#built-with)
  - [Key Features](#key-features)
  - [📊 Sample Outputs](#sample-outputs)
- [💻 Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
  - [Install](#install)
  - [Usage](#usage)
- [👥 Authors](#authors)
- [🔭 Future Features](#future-features)
- [🙏 Acknowledgements](#acknowledgements)
- [📝 License](#license)

---

# 📖 Renewables Ninja ; Solar and Wind Generation Analysis <a name="about-project"></a>

> A Python data project fetching, analysing and visualising real hourly 
> solar PV and wind power generation data for any location in the world 
> using the Renewables Ninja API.

This project connects to the Renewables Ninja API ; powered by NASA MERRA2 
reanalysis data ; to retrieve hourly generation profiles for solar PV and 
wind turbines at any specified location. It analyses seasonal patterns, 
compares solar vs wind output, computes capacity factors, and visualises 
results using both matplotlib and Plotly.

**Key formula:**
``` Capacity Factor (%) = (Actual Energy Output / Maximum Possible Output) × 100 ```

## 🛠 Built With <a name="built-with"></a>

### Tech Stack

- **Language:** Python 3.13
- **Libraries:** requests, json, geopy, pandas, matplotlib, plotly
- **Data Source:** Renewables Ninja API ; NASA MERRA2 reanalysis dataset
- **Environment:** Jupyter Notebook (VS Code)

### Key Features <a name="key-features"></a>

- **Location input** : user types any city ; geopy automatically 
  converts it to latitude and longitude coordinates
- **API integration** : authenticates with Renewables Ninja API using 
  a token and fetches hourly solar PV and wind generation data
- **Solar PV configuration** : customisable tilt, azimuth, tracking 
  type, system loss and capacity parameters
- **Wind turbine configuration** : customisable hub height and 
  turbine model (Vestas V80 2000)
- **Seasonal analysis** : monthly and seasonal generation patterns 
  for both solar and wind
- **Capacity factor analysis** : measures actual output as a 
  percentage of theoretical maximum
- **Location comparison** : compares generation profiles across 
  multiple locations
- **Interactive visualisations** : Plotly charts with hover tooltips 
  showing hourly generation details

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📊 Sample Outputs <a name="sample-outputs"></a>

![Solar vs Wind Generation](assets/solar_wind_comparison.png)

![Monthly Generation Profile](assets/monthly_generation.png)

![Capacity Factor Chart](assets/capacity_factor.png)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📈 Key Findings <a name="key-findings"></a>

*To be updated after analysis is complete.*

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 💻 Getting Started <a name="getting-started"></a>

### Prerequisites

- Python 3.x installed on your machine
- VS Code with the Jupyter extension installed
- A free Renewables Ninja account and API token
  ; sign up at https://www.renewables.ninja

### Setup

Clone this repository:
```sh
git clone https://github.com/NATASHA-ct/renewables-ninja-solar-wind-analysis.git
cd renewables-ninja-solar-wind-analysis
```

### Install

Install all dependencies:
```sh
pip install -r requirements.txt
```

### Usage

1. Sign up at https://www.renewables.ninja and generate your API token
2. Add your token to the notebook where indicated
3. All notebooks are in the `notebooks/` folder. Open and run in order:

| Notebook | Description |
|---|---|
| 01_fetch_solar_wind_data.ipynb | Fetch hourly solar and wind data for any location |
| 02_seasonal_analysis.ipynb | Monthly and seasonal generation patterns |
| 03_capacity_factor_analysis.ipynb | Capacity factor computation and comparison |
| 04_location_comparison.ipynb | Compare generation profiles across locations |

Run all cells from top to bottom using **Run All**.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 👥 Authors <a name="authors"></a>

👤 **Natasha Chirombe**

- GitHub: [@NATASHA-ct](https://github.com/NATASHA-ct)
- LinkedIn: [Natasha Chirombe](https://www.linkedin.com/in/natashatatendachirombe/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 🔭 Future Features <a name="future-features"></a>

- [ ] Build a Streamlit dashboard with interactive location input
- [ ] Add PVGIS data comparison alongside Renewables Ninja results
- [ ] Apply analysis to North Cyprus for thesis validation
- [ ] Add battery storage dispatch modelling on top of generation profiles

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

## 📝 License <a name="license"></a>

This project is [MIT](./LICENSE) licensed.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
