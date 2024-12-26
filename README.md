# ML---SoMiHo-team
Here is a presentation of a process of researching, approaching and solving the Child Mind Institute — Problematic Internet Use - a machine learning competition on the Kaggle platform.
https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use.

This is our first time participating in a kaggle competition so we were quite surprised to see ourselves ranked 58th in the private leaderboard.

Version description:

**Version 2:** first version, only simple data processing (missing data processed by 2 fill functions), only using RandomForestClassifier algorithm. Score 0.266 public/0.247 private.

**Version 3:** add time series data. Score 0.266 public/0.247 private.

**Version 11:** use 3 algorithms: RandomForest, XGBoost, CatBoost (all are classifiers). Score 0.293 public/0.356 private.

**Version 13:** use 3 boosting algorithms: XGBoost, LightGBM, CatBoost (all are regressors). Combined by weighted average. Score 0.386 public/0.386 private.

**Version 15:** indirect learning: learn to predict PCIAT-PCIAT_Total, then convert this value to sii. Score 0.364 public/0.312 private.

**Version 18:** more detailed data processing, applying time series data compression to reduce data dimensionality to help the model learn better. Score 0.412 public/0.441 private.

**Version 19:** only using model 1 (described below) but ensemble is equal to weighted average. Score 0.403 public/0.458 private.

**Version 20:** has model 1, model 2, model 3
  
  Model 1 is still the model of version 18 but: uses time series, uses Season columns, uses voting regressor to ensemble, the objective function is Total then converted to sii
  
  Model 2: still uses 3 algorithms lgbm, xgb, catboost. No time series data, but Season columns are used, the objective function is Total then converted to sii, using voting regressor combined with stacking (nested ensemble)
  
  Model 3: using additional Random Forest, Gradient Boost, learning sii directly, using time series data, removing Season data -> however, this model has not been tested for performance due to no more     submissions.

**Version 22: only using model 2, this is the version with the highest score. Score 0.405 public/0.460 private.**
https://www.kaggle.com/code/lvhoangg2004/notebookeb19475bf7?scriptVersionId=213890303
