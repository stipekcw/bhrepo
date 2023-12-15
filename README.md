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
       a. wc_trial_run_v6_cv.py - ingests cities along the West Coast of the United States, optimizes the hyper-parameters, and does a train test split and cross-validation
      b. 
    - Compared against current state of the art (LiDAR) and Microsoft (Satellite)

