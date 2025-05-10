# **SF Crime Forecasting – CS133 Final Project**

This project was completed for **CS133: Introduction to Data Visualization** at San Jose State University.  
 We analyzed and predicted crime patterns in San Francisco using police incident reports from **2018 to 2025\.** The focus was on **forecasting hourly crime counts** and visualizing crime trends across neighborhoods and time periods.

---

**Team Members**

* Ruiyuan Li

* Tang, Ho Lam (Zeth)

---

## **🎯 Project Objectives**

* Predict **hourly crime counts** using machine learning

* Visualize **spatial and temporal crime patterns** to identify key trends

* Highlight insights on crime hotspots, peak times, and seasonal shifts

---

## **🗂️ Files Included**

* SF\_Crime\_Forecasting.ipynb — Main notebook (Colab-ready)

* SF\_Crime\_Forecasting\_Report.pdf — Full project report

* SF\_Crime\_Forecasting\_Presentation.pdf — Slide deck (10+ slides)

**Run the Notebook**  
 Open SF\_Crime\_Forecasting.ipynb in Google Colab. The notebook performs:

* Data cleaning & preparation

* Feature engineering (time-based features: hour, day, month, year)

* Aggregation of crime counts by hour and location

* Regression modeling:

  * Linear Regression

  * Decision Tree Regressor

  * Random Forest Regressor

* Evaluation using MAE, RMSE, R²

* Visualizations:

  * Heatmaps

  * Bar charts

  * Line charts

## **Dataset Source**

**Police Department Incident Reports (2018–Present)**

[**https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about\_data**](https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about_data)

## 

## 

### **Best Model** 

Based on accuracy and F1-scores, RandomForest is the best-performing model, achieving 79% accuracy and the highest scores across all classes.

### **Key Insights**

**Crime Hotspots Identified:**

Using DBSCAN clustering, we identified major crime hotspots, with Cluster 0 (likely Mission/Tenderloin) showing the highest density of incidents.

**Hourly Crime Patterns:**

Crime counts peaked between noon and early evening, especially in the largest clusters, confirming clear temporal trends in crime activity.

**Effective Parameter Tuning:**

The K-Distance graph was crucial for selecting the best eps value, ensuring DBSCAN produced meaningful clusters rather than noise.

**Spatial vs. Temporal Patterns:**

Our analysis highlighted that different clusters not only vary in location but also show unique hourly crime behaviors, providing deeper insight into crime dynamics.

**Challenge of Imbalanced Data:**

Crime incidents were heavily imbalanced across categories and neighborhoods, emphasizing the need for careful model evaluation and interpretation.

**Clustering Helps Visualization:**

Visualizing the spatial clusters and hourly patterns made complex data easier to understand and offered actionable insights for public safety planning.

## 

## 

## **Challenges**

* Parameter Tuning for DBSCAN:  
  Choosing the optimal eps value was tricky. We used a K-Distance Graph to guide our selection, but it required trial and error to correctly interpret the elbow point.  
* Data Imbalance:  
  Some crime categories and clusters had very few data points, making it difficult to build balanced and accurate models.  
* Finding the Right Approach:  
  One of the biggest challenges was figuring out the best way to approach the problem. We explored different clustering methods, visualizations, and machine learning models before deciding what was most effective for our data.


