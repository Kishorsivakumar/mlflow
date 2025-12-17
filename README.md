##MLFLOW Experiments

import dagshub
dagshub.init(repo_owner='Kishorsivakumar', repo_name='mlflow', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)