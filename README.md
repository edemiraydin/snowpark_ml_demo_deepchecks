# snowpark_ml_demo_deepchecks

Disclaimer: This is experimental. 

I have been exploring DeepChecks, a new open source Python utility for ML testing and validation. In this demo, I used and existing Snowpark Python demo (https://github.com/Snowflake-Labs/snowpark-python-demos/tree/main/Predict%20Customer%20Spend) to predict customer spend and added DeepChecks functions to evaluate data, train and test datasets as well as model. 

The code includes Python Stored Procedures to run DeepChecks natively in Snowflake on the server side. Please note that some dependencies are not currently in the Snowflake Anaconda repository so we had to add them using session.add_import() so they get serialized to run on the server side. 


