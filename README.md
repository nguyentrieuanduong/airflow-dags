# airflow-dags

## Guide

https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-env-variables.html and https://docs.aws.amazon.com/mwaa/latest/userguide/best-practices-tuning.html
https://docs.aws.amazon.com/mwaa/latest/userguide/working-dags-dependencies.html and https://docs.aws.amazon.com/mwaa/latest/userguide/best-practices-dependencies.html
https://docs.aws.amazon.com/mwaa/latest/userguide/using-startup-script.html and https://docs.aws.amazon.com/mwaa/latest/userguide/samples-dbt.html
https://docs.aws.amazon.com/mwaa/latest/userguide/configuring-dag-import-plugins.html

https://airflow.apache.org/docs/apache-airflow/2.10.3/best-practices.html

https://airflow.apache.org/docs/apache-airflow/2.10.3/templates-ref.html
https://airflow.apache.org/docs/apache-airflow/2.10.3/howto/notifications.html
https://airflow.apache.org/docs/apache-airflow/2.10.3/tutorial/taskflow.html
https://airflow.apache.org/docs/apache-airflow/2.10.3/authoring-and-scheduling/dynamic-task-mapping.html
https://airflow.apache.org/docs/apache-airflow/2.10.3/authoring-and-scheduling/deferring.html
https://airflow.apache.org/docs/apache-airflow/2.10.3/authoring-and-scheduling/datasets.html

https://airflow.apache.org/docs/apache-airflow/2.10.3/authoring-and-scheduling/plugins.html#when-are-plugins-re-loaded

## Project structure

```text
.
├── config/                                         # Configurations
├── dags/
│   ├── .airflowignore                              # DAG discovery ignore patterns
│   ├── airflow_dags/
│   │   ├── common/                                 # Shared DAG helper placeholders
│   │   ├── hooks/                                  # Custom hook package placeholder
│   │   ├── operators/                              # Custom operator package placeholder
│   │   └── sensors/                                # Custom sensor package placeholder
│   └── sql                                         # SQL scripts
├── plugins/
│   └── triggers/                                   # Trigger package placeholder
├── scripts/                                        # Custom scripts
├── tests/
│   └── integration/                                # Integration test package placeholder
│   └── unit/                                       # Unit test package placeholder
├── requirements.txt                                # Airflow 2.10.3 / Python 3.11 constraint URL
├── mwaa-constraints-airflow_2.10.3-python_3.11.txt # Local constraints snapshot
└── startup.sh                                      # Node startup script
```
