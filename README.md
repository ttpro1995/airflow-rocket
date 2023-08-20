# Run airflow in offline mode

## First time setup
We only need to do once for each project

We set environment variable to project folder

```
export AIRFLOW_HOME=/home/lap60728/workspace/study/airflow_rocket
export AIRFLOW__CORE__LOAD_EXAMPLES=False 
```

Then run init in same terminal. The environment variable above must be set succesfully 

```
airflow db init # run once
```

Create first user
```
airflow users create --username admin --password admin --firstname Anonymous --lastname Admin --role Admin --email admin@example.org
```

To run airflow, open two separate terminal. Each terminal have to set AIRFLOW_HOME variable.  

```
airflow webserver
```

Then 

```
airflow scheduler
```