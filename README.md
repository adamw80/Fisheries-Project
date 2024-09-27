# Global Patterns of Transshipment Behavior Analysis

## Project Overview

This project aims to analyze global patterns of transshipment behavior, particularly focusing on illegal fishing activities. Illegal fishing is a significant threat to marine biodiversity and the sustainability of global fish stocks, impacting both the environment and the livelihoods of communities dependent on fishing. The project uses data science and machine learning techniques to explore, analyze, and predict illegal transshipment and loitering events involving fishing vessels.

### Key Objectives:

1. **Identify Key Players in Illegal Fishing:**
   - Determine the countries and vessels most involved in illegal fishing activities.
   
2. **Analyze Spatial and Temporal Patterns:**
   - Understand the movement and behavior of transshipment vessels and their encounters with other vessels.
   
3. **Predict Future Encounters:**
   - Utilize machine learning models to forecast future encounters between fishing vessels and transshipment vessels.

4. **Assess Legal Boundaries:**
   - Predict the likelihood of vessels operating within Exclusive Economic Zones (EEZs) illegally.

## Project Structure

### 1. Data Exploration
- **Data Loading & Description:** Load multiple datasets on transshipment, loitering events, and encounters, and understand their structure and contents.
- **Initial Data Analysis:** Explore basic statistics and visualize the distribution and frequency of events.

### 2. Exploratory Data Analysis (EDA)
- **Identify Major Players:** Determine the countries and vessels involved in illegal fishing.
- **Spatial and Temporal Analysis:** Analyze the movements and encounters of vessels over time and across different regions.

### 3. Machine Learning Models

#### Classification and Prediction
- **Model Preparation:** Data preprocessing, including scaling, encoding, and imputation for machine learning models.
- **Classification Models:** Implement RandomForestClassifier to classify vessels based on their behavior and predict future encounters.
- **Anomaly Detection:** Use IsolationForest to detect unusual patterns in vessel movements.

#### Forecasting Vessel Movements
- **LSTM Models:** Use Long Short-Term Memory (LSTM) models to forecast vessel movements and predict their locations.
- **Evaluation Metrics:** Evaluate model performance using accuracy, classification reports, confusion matrix, and mean squared error.

### 4. Network Analysis
- **Community Detection:** Apply community detection algorithms like Louvain to identify clusters of vessels involved in illegal activities.
- **Graph Analysis:** Utilize network analysis tools to visualize relationships and connections between vessels.

### 5. Visualization and Mapping
- **Geospatial Visualization:** Use Folium and Cartopy for visualizing vessel movements, encounters, and hotspots.
- **Heatmaps:** Generate heatmaps of loitering and transshipment events to identify areas of high activity.

### 6. Prediction and Visualization
- **Forecasting Hotspots:** Predict areas with high probabilities of illegal activities based on historical data.
- **Visual Representation:** Create interactive maps and visualizations to illustrate patterns and predictions.

### 7. Final Analysis
- **Summary of Findings:** Discuss key insights, implications for enforcement, and potential policy recommendations.

## Dependencies

The project requires the following libraries:

- **Data Handling:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `folium`, `geopandas`, `cartopy`
- **Machine Learning:** `scikit-learn`, `tensorflow`
- **Network Analysis:** `networkx`, `community`
- **Miscellaneous:** `warnings`

To install all dependencies, run:
```bash
pip install pandas numpy matplotlib folium geopandas scikit-learn tensorflow networkx community cartopy shapely
```

## Usage

1. **Load the Data:**
   Place the datasets (`transshipment-vessels.csv`, `loitering-events.csv`, `encounter-events.csv`) in the designated directory and run the notebook cells to load and preprocess the data.

2. **Run the Analysis:**
   Follow the sequential steps in the notebook to perform EDA, machine learning modeling, and network analysis.

3. **Visualize the Results:**
   Use the visualization sections to view vessel movements, encounter patterns, and predicted hotspots.

4. **Model Predictions:**
   Experiment with different models and parameters to optimize predictions for vessel movements and illegal activities.

## Dataset

The datasets used in this project include records of transshipment vessels, loitering events, and encounters, detailing attributes such as vessel ID, location, time, and behavior. The data provides a comprehensive overview of global fishing activities and their compliance with maritime boundaries.

## References

1. Global Fishing Watch - [Fishing Data](https://globalfishingwatch.org/)
2. Scikit-learn Documentation - [Scikit-learn](https://scikit-learn.org/)
3. TensorFlow Documentation - [TensorFlow](https://www.tensorflow.org/)
4. NetworkX Documentation - [NetworkX](https://networkx.org/)

## Acknowledgments

This project is developed as part of an effort to understand and mitigate illegal fishing activities. Special thanks to Global Fishing Watch for providing access to the transshipment and loitering datasets.
