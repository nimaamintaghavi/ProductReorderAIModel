<!-- TABLE OF CONTENTS -->
<div id="toc_container">
<p class="toc_title">Table of Contents</p>
    <li><a href="#About The Project">1 - About The Project</a></li>
    <li><a href="#Services and Algorithm Used">2 - Services and Algorithm Used</a></li>
    <li><a href="#Required Packaged">3 - Required Packaged</a></li>
</div>


## About The Project
InstaS'Mart, a new online grocery ordering service,  would like to find the customers that will likely re-order their products. 


This project will help the company with creating a buy again section on their website featuring products that 

have a high likelihood of being purchased again by a particular customer based on that customer's purchase history. The overall goal is to increase sales and profit by reducing the opportunity the customer has to hesitate when seeking out grocery products and making a purchase. An increase in sales resulting from the clicking the buy again section will constitute the measurable increase in effectiveness. 

The source data is part of a Kaggle challenge and can be downloaded at the link below: 
https://www.kaggle.com/yasserh/instacart-online-grocery-basket-analysis-dataset 

There are five distinct files:

| Table Name    | Records      |
|---------------|--------------|
|aisles         | 134          |
|departments    | 21           |
|order_products | 32.4 million |
|orders         | 3.4 million  |
|products       | 50 thousand  |

All files are .csv files.
Each file will be given its own folder to be read into AWS Athena.
Tables will then be made for each file for purposes of data analysis. 

## Services and Algorithm Used

AWS Sagemaker Service will be utililzed to create a machine learning model.

Machine Learning <b>Model</b> will be `xgboost classifier`

The model will be <b>trained</b> on `instance_count = 1` and `instance_type = 'ml.m5.xlarge'`

<b>Predictions</b> will be done on `initial_instance_count = 3` and `instance_type = 'ml.m5.xlarge'`



## Required Packaged
Python 3.9 relase will be used with the following packages:

| Package | Version |
|---------------|---------|
|awswrangler    | 2.15.1  |
|boto3          | 1.20.23 |
|matplotlib     | 3.1.3   |
|numpy          | 1.21.6  |
|pandas         | 1.0.1   |
|pyathena       | 2.1.0   |
|sagemaker      | 2.70.0  |
|seaborn        | 0.10.0  |


