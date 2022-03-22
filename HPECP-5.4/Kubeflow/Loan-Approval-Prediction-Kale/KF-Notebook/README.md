# Steps:
* Execute Prerequisites.ipynb.

## Execute the kubeflow Pipeline
   
   * **When SSL is enabled on Platfrom.**<br>
    Execute Loan-Approval-Prediction-MinIO-SSL.ipynb.
   
   * **When SSL is not enabled on Platfrom.**<br>
    Execute Loan-Approval-Prediction-MinIO-NoSSL.ipynb.
   
   Get the best model path from Kubeflow.<br>
   ![](images/BestModelS3.PNG)
   
## Register the Model in Platform Model Registry.
   
   * **Register new mode in Model Registry.**<br>
   ![](images/RegisterModel.PNG)

## Deploy the Model

   * **Deploy the model from Model Serving.**<br>
   ![](images/DeployModel1.PNG)

   Edit the yaml and add secret and proxy var as env.<br>
   ![](images/DeployModel2.PNG)

## Prediction

   * **When SSL is enabled on Platfrom.**<br>
   Execute the Prediction-SSL.ipynb

   * **When SSL is not enabled on Platfrom.**<br>
   Execute the Prediction-NoSSL.ipynb
