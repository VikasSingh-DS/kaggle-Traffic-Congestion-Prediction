# Traffic-Congestion-Prediction-Feature-Engineering-and-LightGBM
The dataset for this competition includes aggregate stopped vehicle information and intersection wait times. Your task is to predict congestion, based on an aggregate measure of stopping distance and waiting times, at intersections in 4 major US cities: Atlanta, Boston, Chicago & Philadelphia.

# Objective
* Exploratory Data Analysis (EDA) to analyzing data sets to summarize their main characteristics, often with visual methods.
* Extensive feature engineering and modeling.

# Data Description
The data consists of aggregated trip logging metrics from commercial vehicles, such as semi-trucks. The data have been grouped by intersection, month, hour of day, direction driven through the intersection, and whether the day was on a weekend or not.

For each grouping in the test set, you need to make predictions for three different quantiles of two different metrics covering how long it took the group of vehicles to drive through the intersection. Specifically, the 20th, 50th, and 80th percentiles for the total time stopped at an intersection and the distance between the intersection and the first place a vehicle stopped while waiting. You can think of your goal as summarizing the distribution of wait times and stop distances at each intersection.

Each of those six predictions goes on a new row in the submission file. Read the submission TargetId fields, such as 1_1, as the first number being the RowId and the second being the metric id. You can unpack the submission metric id codes with submission_metric_map.json.

The training set includes an optional additional output metric (TimeFromFirstStop) in case you find that useful for building your models. It was only excluded from the test set to limit the number of predictions that must be made.

You can also access the data through BigQuery at https://bigquery.cloud.google.com/dataset/kaggle-competition-datasets:geotab_intersection_congestion once you have followed the instructions in BigQuery-Dataset-Access.md. The instructions are stored in that file to ensure that people who access the dataset on BigQuery have accepted the competition rules. Republishing the instructions, including on kaggle forums, is grounds for disqualification from the competition.

# Overview
We’ve all been there: Stuck at a traffic light, only to be given mere seconds to pass through an intersection, behind a parade of other commuters. Imagine if you could help city planners and governments anticipate traffic hot spots ahead of time and reduce the stop-and-go stress of millions of commuters like you.

Geotab provides a wide variety of aggregate datasets gathered from commercial vehicle telematics devices. Harnessing the insights from this data has the power to improve safety, optimize operations, and identify opportunities for infrastructure challenges.

The dataset for this competition includes aggregate stopped vehicle information and intersection wait times. Your task is to predict congestion, based on an aggregate measure of stopping distance and waiting times, at intersections in 4 major US cities: Atlanta, Boston, Chicago & Philadelphia.

This competition is being hosted in partnership with BigQuery, a data warehouse for manipulating, joining, and querying large scale tabular datasets. BigQuery also offers BigQuery ML, an easy way for users to create and run machine learning models to generate predictions through a SQL query interface.

Kaggle recently released a BigQuery integration within our kernels notebook environment, and this starter kernel gives you a great starting point for how to use BQ & BQML. You’re encouraged to use your data savvy, resourcefulness & intuition to find and join in additional external datasets that will increase your models’ predictive power.

Alright, stop waiting and get started!

# Acknowledgments
Geotab

A big thanks to Geotab for providing the dataset for this competition! Geotab is advancing security, connecting commercial vehicles to the internet and providing web-based analytics to help customers better manage their fleets. Geotab’s open platform and Marketplace, offering hundreds of third-party solution options, allows both small and large businesses to automate operations by integrating vehicle data with their other data assets. As an IoT hub, the in-vehicle device provides additional functionality through IOX Add-Ons. Processing billions of data points a day, Geotab leverages data analytics and machine learning to help customers improve productivity, optimize fleets through the reduction of fuel consumption, enhance driver safety, and achieve strong compliance to regulatory changes. Geotab’s products are represented and sold worldwide through Authorized Geotab Resellers. To learn more, please visit www.geotab.com and follow us @GEOTAB(https://twitter.com/GEOTAB) and on LinkedIn(https://www.linkedin.com/company/geotab/).

