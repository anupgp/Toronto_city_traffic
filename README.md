# Giospatial Data analysis project - Working 

# Visualizing traffic on the streets of Toronto
In this project, I aim to hone my skills with analyzing and visualizing geospatial data to tell a story


## ✅ Purpose & Overview
The objective of this project is to:
- Develop an interactive plot to visualize giospatial data
- Identify significant traffic congestion areas in Toronto city.
- Provide intuitive visualizations to support model interpretability for both technical and non-technical audiences.

## Dataset Overview 
The City of Toronto's Transportation Services Division collects short-term traffic count data across the City on an ad-hoc basis to support a variety of safety initiatives and projects....
More information: [Traffic Volumes - Multimodal Intersection Turning Movement Counts](https://ckan0.cf.opendata.inter.prod-toronto.ca/dataset/traffic-volumes-at-intersections-for-all-modes)

Data Source: [Download](https://ckan0.cf.opendata.inter.prod-toronto.ca/dataset/traffic-volumes-at-intersections-for-all-modes/resource/262469c2-abfe-4756-9068-4ea5c7ba1af7)  
Resources: *fedesoriano*, [Open Data Toronto City](https://www.toronto.ca/city-government/data-research-maps/open-data/learning-resources/)


## 📊 Key Variables & Feature Descriptions
| Column Name       | Description                                                                                         |
|-------------------|-----------------------------------------------------------------------------------------------------|
| count_id          | Unique identifier for each count.                                                                   |
| count_date        | Date the count was conducted. For Turning Movement Counts, studies are conducted on 1 day.          |
| location_name     | Human-readable name of the location where the count was conducted                                   |
| longitude         | Longitude GPS coordinate                                                                            |
| latitude          | Latitude GPS coordinate                                                                             |
| centreline_type   | Intersection node or Midblock segment.                                                              |
| centreline_id     | Unique location identifier that corresponds to the Toronto Centreline or Intersection File datasets.|
| start_time        | Start time of the 15-minute interval                                                                |
| end_time          | End time of the 15-minute interval                                                                  |
| px                | If there is a traffic control signal at the location, this is the unique identifier for the signal. |
| n_appr_cars_r     | Volume of cars that enter the intersection from the north leg (approach), in a southbound direction of travel, and make a right turn.|
| n_appr_cars_t     | Volume of cars that enter the intersection from the north leg (approach), in a southbound direction of travel, and continue through. |


## 🔍 Exploratory Data Analysis

### Key trends and insights:
- **Age**: Normally distributed across the population.  
- **Sex Distribution**: Majority male, indicating gender imbalance.  
- **Chest Pain Type**: Most common is 'ASY' (Asymptomatic).  
- **Feature Correlation**: Oldpeak and ST_Slope show notable associations with heart disease.



**Figure 1.**
![Visualization of Toronto city intersections (data collection points) on a map](toronto_traffic_1.html)


## 🧠 Data Visualization

Developed Visualizations:
- Plotly Scatter map for basic geospatial visualization
- Matplotlib plots for ploting timeseries data 

## 🎨 Data Visualization Objectives

1. **Explore the distribution of street intersections in Toronto City**
    - Giospatial visualization

2. **Examine the average traffic across time**  
   - Timeseries plots

## 🎯 Audience

This project is designed for:

- **Anyone interested in Toronto city traffic across days and time

## 📚 Tech Stack & Libraries

| Library        | Purpose                                  |
|----------------|------------------------------------------|
| `pandas`       | Data manipulation                        |
| `numpy`        | Numerical computations                   |
| `seaborn`, `matplotlib`| Data visualization                 |
| `plotly`, `Dash` | Interactive GIS plots |


## Ethical Considerations

- The dataset is publicly available for anyone to use.

## Future Enhancements

- Implement more informative plots.  
- Perform classification of traffic intersections

## References

- **City of Toronto's Open data**: https://www.toronto.ca/city-government/data-research-maps/open-data/learning-resources/
