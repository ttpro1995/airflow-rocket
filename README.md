export AIRFLOW_HOME=/home/lap60728/workspace/study/airflow_rocket

airflow db init # run once

airflow users create --username admin --password admin --firstname Anonymous --lastname Admin --role Admin --email admin@example.org