# Airflow

## Basic concept

1. DAGs: 1) Sensor 2) Operator

### Main components

- **Scheduler** plans the execution of jobs based on a trigger or schedule.
- **Work queue** is used by **Scheduler** to deliver tasks that need to be run to the Workers.
- **Worker**(ECRs) executes the operation defined in each *DAG*. Usually, a **Worker** pull its task from **Work queue** when it is ready to process a task. When it completes the execution of the task, it will attempt to process more work from the **Work queue** until no task exists. When work in the queue arrives, the worker will begin to process it.
  In ***multi-node airflow architecture***, daemon processes are distributed across all worker nodes. The web server and scheduler are installed at the master node, and workers would be installed at each different worker nodes. To this mode of architecture, Airflow has to be configured with *CeleryExecutor*(TODO: What is this?).
- **Database** saves credentials, connections, history, and configuration. The database, often referred to as the metadata database, also stores the state of all tasks in the system.
- **Web Interface** provides a control dashboard for users and maintainers. The web interface is built using the *Flask* web-development micro-framework.

Data Partitioning: Pipeline data partitioning is the process of isolating data to be analyzed by one or more attributes, such as time, logical type, or data size. And it often leads to faster and more reliable pipelines.

Data Lineage: The data lineage of a dataset describes the discrete steps involved in the creation, movement, and calculation of that dataset. Describing and servicing data lineage is one of the key ways we can ensure that everyone in the organization *has access to and understands where data originates and how it is calculated*.

## Big company examples

### Twitter

- Situation
  - ~400 DAG files
  - ~30 customer teams
  - [ ETL --> Train model --> Test model --> Push model ] Under Airflow  --> Production model deployment system
- Airflow pain points
  - Development speed.
  - Clunky interface

### Airbnb

### Netflix



### REF

- [Data pipeline using apache airflow](https://medium.com/@abinmj656/data-pipeline-using-apache-airflow-81e47f3d9271)

- [Data pipeline using airflow: ](https://medium.com/swlh/data-pipelines-with-apache-airflow-46258deb2844)

- [Airflow design principles: multi-tenant vs monolithic architecture](https://www.astronomer.io/blog/airflow-infrastructure)

  