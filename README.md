# Linear Regression Demo with Snowpark Python and DeepChecks

Disclaimer: This is experimental. 

I have been exploring DeepChecks, a new open source Python utility for ML testing and validation. In this demo, I used and existing Snowpark Python demo (https://github.com/Snowflake-Labs/snowpark-python-demos/tree/main/Predict%20Customer%20Spend) to predict customer spend and added DeepChecks functions to evaluate data, train and test datasets as well as model. 

The code includes Python Stored Procedures to run DeepChecks natively in Snowflake on the server side. Please note that some dependencies are not currently in the Snowflake Anaconda repository so we had to add them using session.add_import() so they get serialized to run on the server side. 


The demo uses DeepCheck v0.8 that has dependencies to the following packages: https://libraries.io/pypi/deepchecks/0.8.0

albumentations>=1.1.0category-encoders>=2.3.0dataclasses>=0.6imagehash>=4.0.0imgaug>=0.4.0importlib-resources>=1.3ipykernel>=4.10.1ipython<8,>=5.5.0 ipywidgets>=7.5.0jsonpickle>=2matplotlib>=3.3.4numpy>=1.19opencv-python<4.6.0.66,>=4.5.5.62pandas>=1.1.5plotly==5.5.0PyNomaly>=0.3.3pytorch-ignite>=0.4.8requests>=2.22.0scikit-learn>=0.23.2scipy>=1.4.1seaborn>=0.1.0statsmodels>=0.11.0tqdm>=4.62.3typing-extensions>=3.7.4.3

Medium post: https://medium.com/snowflake/using-deepchecks-for-monitoring-data-and-model-drift-in-snowflake-f1d4d872322
