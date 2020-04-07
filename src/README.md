Stores source code (python, R etc) which serves multiple scenarios. During data exploration and model training, we have to transform data for particular purpose. We have to use same code to transfer data during online prediction as well. So it better separates code from notebook such that it serves different purpose.

* `data`: Scripts to download or generate data 
* `features`: Scripts to turn raw data into features for modeling
* `models`: Scripts to train models and then use trained models to make predictions