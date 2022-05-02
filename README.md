# Satellite_pmPredict
## Machine learning approaches to predict PM<sub>2.5</sub> using satellite images

Author: Xinyu (Sindy) Du

Advisor: Dr. Roger D. Peng

Secondary Reader: Dr. Abhirup Datta

*Department of Biostatistics*

*Johns Hopkins Bloomberg School of Public Health*



## Description

According to World Health Organization, air pollution is considered to be one of the greatest environmental health threats. PM<sub>2.5</sub>, fine particles with a diameter that is generally 2.5 micrometers and smaller, is inhalable into the lungs and can induce adverse health effects. In order to mitigate the effects of PM<sub>2.5</sub> on health outcomes, it is crucial to make accurate predictions of ambient concentrations. In the past, most studies developed traditional linear models from meteorological data or Environmental Protection Agency (EPA) ambient air quality monitors. However, the non-linear relationship between PM<sub>2.5</sub> and other factors impacts the effectiveness of the models. Another barrier is the sparseness of air quality monitors and the limited data sources, which also hinder researchers’ ability to get accurate predictions. Recently, advanced technologies in satellite remote sensing have been widely used to estimate PM<sub>2.5</sub> concentrations. The implementation of machine learning approaches has improved computational efficiency and accuracy.

In this study, we used daily satellite imagery from January 2017 to October 2021 in 25 U.S. locations, and implemented an eXtreme Gradient Boosting (XGBoost) algorithm, a deep Convolutional Neural Network (CNN), and a CNN-XGBoost pipeline to make predictions based on the extracted features from each satellite image and atmospheric information along with meteorological conditions. To evaluate the performance of each model, we used daily EPA Federal Reference Method PM2.5 measurements as the validation data, and calculated the corresponding root mean squared error (RMSE) and the coefficient of determinant (R<sup>2</sup>). After combining each daily observation from 25 locations, the XGBoost approach demonstrated the highest performance with an RMSE of 3.98 μg m<sup>-3</sup> and an R<sup>2</sup> of 0.65. The CNN-XGBoost pipeline, tending to overestimate PM<sub>2.5</sub> concentrations, had an RMSE of 5.87 μg m<sup>-3</sup> and an R<sup>2</sup> of 0.37. In conclusion, our study showed that XGBoost achieved reasonable PM<sub>2.5</sub> prediction performance, indicating that the application of satellite remote sensing data and machine learning approaches has significant potential use in PM<sub>2.5</sub> concentrations prediction.
