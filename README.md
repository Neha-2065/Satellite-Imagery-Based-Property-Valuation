# Satellite-Imagery-Based-Property-Valuation
Satellite imagery + tabular data for house price prediction
Made a model that uses satellite images plus regular house data to predict prices.

## Results
Dataset: 16K training houses, 5K test houses (21 features + satellite images each)
Random Forest baseline got around $128K RMSE error
Built CNN with ResNet18 that combines image + table data

## Files
1. data_fetcher_ipnyb.ipynb - downloads all satellite images from mapping service
2. preprocessing.ipynb - loads data + builds baseline Random Forest model  
3. model_training-2.ipynb - trains CNN using images + house features

### How to run
Upload train1.xlsx and test2.xlsx files to Colab
Run data_fetcher first (gets ~21K satellite images)
Run preprocessing (combines data + trains baseline model, RMSE ~$128K)
Run model_training (ResNet18 CNN on images + features)

Dataset has 16K training houses and 5K test houses around Seattle. Main price drivers are house size (sqftliving, 70% correlation) and quality grade (66%). Images show actual lot/ neighborhood.
