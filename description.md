# Crop Yield Prediction

The aim of this data science project is to predict crop yield using the dataset provided from Crop Yield Prediction. The dataset includes various environmental and agricultural factors such as rainfall, temperature, fertilizer usage, and macronutrient levels, along with the corresponding crop yield in Quintals per acre.

## Data Dictionary

 Column Names:
 
 - Rain Fall (mm)  
 - Temperature (C) 
 - Fertilizer (kg) 
 - Nitrogen (N)     
 - Phosphorous (P) 
 - Potassium (K)           
 - Yield (Q/acres)  

## Data Preprocessing

Upon examining the dataset, it was found that the temperature column contained invalid values represented as ":". These entries were removed, and the column was converted to a float data type. Missing values were replaced with the median of their respective columns.

## Exploratory Data Analysis (EDA)
Insights:
- The dataset likely represents two distinct crops, indicated by clusters in graphs of rainfall, temperature, and crop yield.
- Fertilizer usage appears to have a proportional relationship with crop yield, with some exceptions.
- Temperature and rainfall also exhibit distinct patterns possibly corresponding to different crop seasons.
- Macronutrients (Nitrogen, Phosphorus, Potassium) show varying distributions, indicating potential differences in crop requirements.
- Temperature emerges as the most influential factor in predicting crop yield, followed by rainfall.

## Model Building and Evaluation

Two regression models, Decision Tree Regressor and Random Forest Regressor, were trained and evaluated. Random Forest Regressor outperformed Decision Tree Regressor, achieving an R2 score of 0.802 compared to 0.77. Both models indicate the importance of temperature and rainfall in predicting crop yield.

## Conclusion

The dataset represents two distinct crops with varying environmental and agricultural factors influencing crop yield. Temperature emerges as the most significant predictor, followed by rainfall, while fertilizer and macronutrient levels also play a role. The Random Forest Regressor model proves effective in predicting crop yield based on these factors. However, further analysis could explore additional variables and factors impacting crop yield.
