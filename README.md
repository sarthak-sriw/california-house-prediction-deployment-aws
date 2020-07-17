# california-house-prediction-deployment-aws

1. Set up credentials to the cloud service provider . For eg in case of aws go to IAM role and create a role and note down the **key** and **secret key**

2. Enter the credentials of service provider and connect to using **sls config credentials  --provider aws --key ____  --secret ___**

3. Write the following cmd to initialize the handler.py(Lambda Function) and serverless.yml files **sls create --template aws-python3 --name california-housing**

![](california-house-pred/2.PNG)

4. Edit the handler.py and serverless.yml 

![](california-house-pred/Capture.PNG)

5. In hadler.py we need to load the weights we saved earlier 

![](california-house-pred/Capture3.PNG)

6. In order to test the handler.py run the file with do_main() function 

![](california-house-pred/Capture1.PNG)

7. To test the lambda function locally run the following command **sls invoke local --function predict-price --path event.json**   where event.json is created in the previous step

8. Finally deploy the model  using sls deploy

![](california-house-pred/Capture4_LI.PNG)

