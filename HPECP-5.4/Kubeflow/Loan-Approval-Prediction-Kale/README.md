## Prerequistes 
* Create Secret for MLFlow.
    ```
    apiVersion: v1
    kind: Secret
    metadata:
      name: mlflow-secret
      labels:
        kubedirector.hpe.com/secretType: mlflow
    type: Opaque
    data:
      MLFLOW_ARTIFACT_ROOT: czM6Ly9tbGZsb3c= 
      AWS_ACCESS_KEY_ID: YWRtaW4= #admin
      AWS_SECRET_ACCESS_KEY: YWRtaW4xMjM= #admin123
    ```
* Deploy MLFlow Server.
* Create a bucket name **loan-prediction**.
* Upload **train.csv** and **test.csv** in **loan-prediction** bucket.


# For executing form KD Notebook refer [here](KD-Notebook).

# For executing from Kubeflow Notebook refer [here](KF-Notebook).




