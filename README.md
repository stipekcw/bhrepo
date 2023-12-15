# bhrepo
POC: Clinton Stipek - stipekcw@ornl.gov

- To see current workflow please see workflow.PNG

## Getting started

The main objective:

1. To develop a model (Vivaldi) that generates building height from building morphology features 
    - Current state of art is using 162 features (city, block, street level information)
    - Vivaldi is using 30 features from Gauntlet (morphology features derived from footprint information - 65 features)
        - Gauntlet POC: Taylor Hauser - hausertr@ornl.gov
    - Metrics for comparison are Mean Absolute Error (MAE), Root-Mean-Squared Error (RMSE), and Goodness of Fit (R^2)
    - Overall workflow - see workflow.PNG
    - There are 4 different test (3 LiDAR, 1 Satellite)
        - wc_trial_run_v6_cv.py - ingests cities along the west coast of the United States, optimizes the hyper-parameters, and does a train test split and cross-validation
        - ec_trial_run_v6_cv.py - ingests cities along the east coast of the United States, optimizes the hyper-parameters, and does a train test split and cross-validation
        - berlin_run_v6_cv.py - ingests Berlin and trains in France, optimizes the hyper-parameters, and does a train test split and cross-validation
        - city_trial_run_v6_cv.py - ingests 10 cities (select) based on regularized satellite imagery, optimizes the hyper-parameters, and does a train test split and cross-validation
    - Compared against current state of the art (LiDAR) and Microsoft (Satellite)

