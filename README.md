# Porto Taxi Trajectory Analysis & Hotspot Detection

## Project Overview
This project conducts a comprehensive analysis of taxi trajectory data from Porto, Portugal, focusing on identifying spatial and temporal patterns in taxi demand. The analysis combines geospatial data science techniques with interactive visualizations to uncover valuable insights about urban mobility patterns in Porto.

## Dataset
- **Source**: [Taxi Trajectory Data from Kaggle](https://www.kaggle.com/datasets/crailtap/taxi-trajectory)
- **Description**: Contains complete trajectories (anonymized) of 442 taxis running in Porto, Portugal
- **Time Period**: 1.5 million entries from 2013-2014
- **Variables**: GPS coordinates, timestamps, trip IDs, and taxi IDs

## Key Insights

### Temporal Patterns
- **Peak Hours**: Morning (8-10 AM) and evening (3-6 PM) commutes show highest demand
- **Weekly Trends**: Fridays and Saturdays exhibit 30% higher demand compared to weekdays
- **Seasonal Variations**: Noticeable dip in August, with peaks in spring and late fall

### Spatial Analysis
- **Hotspot Identification**: Implemented HDBSCAN clustering to detect high-density pickup areas
- **Key Clusters**: 
  - Major transportation hubs
  - Tourist attractions
  - Nightlife districts
  - Business centers
- **Demand Patterns**: Clear spatial correlation between commercial areas and peak hours

## Technical Implementation

### Methodology
1. **Data Preprocessing**
   - Cleaning and filtering of raw GPS trajectories
   - Coordinate validation and outlier removal
   - Temporal feature extraction

2. **Temporal Analysis**
   - Hourly, daily, and monthly demand patterns
   - Weekday vs weekend comparisons
   - Time-series visualization of demand fluctuations

3. **Spatial Analysis**
   - Geospatial clustering using HDBSCAN
   - Density-based hotspot identification
   - Interactive mapping of clusters

### Technologies Used
- **Core**: Python, Jupyter Notebooks
- **Data Processing**: pandas, NumPy
- **Geospatial**: GeoPandas, HDBSCAN, Shapely
- **Visualization**: Matplotlib, Seaborn, Folium

## Project Structure
```
porto-taxi-clustering/
├── data/                      # Data files
│   ├── raw/                   # Original dataset
│   └── processed/             # Processed data and visualizations
├── notebooks/                 # Jupyter notebooks
│   └── porto_taxi_analysis.ipynb  # Main analysis notebook
└── requirements.txt           # Python dependencies
```

## Getting Started
1. Install dependencies: `pip install -r requirements.txt`
2. Download the dataset from the link above
3. Run the Jupyter notebook: `jupyter notebook notebooks/porto_taxi_analysis.ipynb`

## Future Work
- Integration with OpenStreetMap for point-of-interest analysis
- Predictive modeling of taxi demand
- Interactive web dashboard for exploration
- Comparison with public transportation data

## License
This project is released under the MIT License.

## Acknowledgments
- Dataset provided by [Kaggle](https://www.kaggle.com/datasets/crailtap/taxi-trajectory)
- Built with Python's scientific computing stack
