# california-house-prediction-deployment-aws

1. Set up credentials to the cloud service provider . For eg in case of aws go to IAM role and create a role and note down the **key** and **secret key**

2. Enter the credentials of service provider and connect to using **sls config credentials  --provider aws --key ____  --secret ___**

3. Write the following cmd to initialize the handler.py(Lambda Function) and serverless.yml files ** sls create --template aws-python3 --name california-housing**
![](california-house-pred/2.png)
