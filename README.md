# Diet Planner with unsupervised learning and LLMs

This repository contains code for predicting weight status using the K-means clustering algorithm and generating a diet plan based on the predicted weight status.

## Introduction

This project aims to help individuals understand their weight status and generate a personalized diet plan to maintain or achieve a healthy weight. It utilizes machine learning techniques to predict weight status and recommends a diet plan accordingly.

## Files

- `weight_status_prediction.ipynb`: Jupyter Notebook containing the code for K-means clustering to predict weight status.
- `diet_plan_generation.ipynb`: Jupyter Notebook containing the code for generating a diet plan based on the predicted weight status.
- `data.csv`: Dataset used for weight status prediction.
- `food_data.csv`: Dataset containing food information for generating the diet plan.

## Functions and Modules

### 1. `euclidean_distance(point1, point2)`

   - Calculates the Euclidean distance between two points in a multidimensional space.
   - Used within the K-means clustering algorithm to measure the distance between data points and cluster centroids.

### 2. `assign_points_to_clusters(clusters, data)`

   - Assigns each data point to the nearest cluster centroid based on Euclidean distance.
   - Returns the labels indicating the assigned cluster for each data point.

### 3. `compute_clusters(data, labels, n_clusters)`

   - Computes the new centroids of the clusters based on the mean of the points assigned to each cluster.
   - Returns the updated cluster centroids.

### 4. `kmeans(data, n_clusters, max_iters=1000)`

   - Implements the K-means clustering algorithm to group data points into clusters.
   - Returns the cluster labels and centroids.

### 5. `predict_weight_status(user_data, clusters, cluster_majority_class)`

   - Predicts the weight status of a user based on their input data.
   - Utilizes the K-means clustering model and majority class labels within clusters.

### 6. `diet_plan()`

   - Generates a diet plan based on the predicted weight status.
   - Calculates the average daily calories for each weight status category.
   - Selects food items from a dataset based on calorie content and weight status.
   - Uses a LLM to help make a diet plan.

## Usage

1. Install the required packages using `pip install -r requirements.txt`.
2. Open and run the `Diet_Planner.ipynb` notebook to predict weight status and make a diet plan.
3. Ensure that the `Dataset.csv` file is in the same directory as the notebook.
4. Ensure that the `Food and Calories - Sheet 1.csv` file is in the same directory as the notebook.

## Requirements

- Python 3
- Jupyter Notebook
- Pandas
- Numpy
  (along with other used libraries)

## Contributors

- [Muhammad Hisan Usman](https://github.com/hisanusman)


Feel free to contribute by opening issues or submitting pull requests.
### Disclaimer: The use of this code complies with all governing bodies; however, it should not be used as a substitute for professional medical advice, diagnosis, or treatment. We are not liable for any warranty or liability for your use of this information. ``(USE IN THE PRESENCE OF A DIETICIAN)!``
