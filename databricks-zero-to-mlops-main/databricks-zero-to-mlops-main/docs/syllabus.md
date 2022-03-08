# MLOps from Zero with Databricks

A four week course on MLOps with Spark and Databricks.  By the end of this course, you will be able to develop ML models using standardized workflows for data processing and model management and maintenance using open-source tools.  This is accomplished by using PySpark and MLflow to build scalable and reproducible solutions using MLOps methodologies.

[Course Intro Video](https://drive.google.com/file/d/1j-9NIFiDErluv4mgVWfgXkGiA2jK3Ndp/view?usp=sharing)
[Course Intro Slides](https://docs.google.com/presentation/d/1Outh5yuWk0CBXMpp6JeY0u6aqPJH1ilcMJGPUN_74gc/edit?usp=sharing)
## Logistics

* Two Three-Hour Weekly Sessions
* Use [Azure Open Datasets](https://docs.microsoft.com/en-us/azure/open-datasets/dataset-catalog#AzureDatabricks)

## Week by Week Schedule

### Week One:  Getting Started with Spark for MLOPs

#### Topics

* Topic:  Getting Started with Databricks and Spark
* Topic:  Getting Started with Continuous Integration

#### Learning Objectives

*   Compose Continuous Integration solutions
*   Compose Databricks/Spark Cluster Solutions
*   Evaluate best practices for PySpark software engineering

#### Part A Workshop

* [Getting Started with Databricks and Spark](https://github.com/FourthBrain/databricks-zero-to-mlops/blob/main/docs/week1-notes.md#workshop-a--getting-started-with-databricks-and-spark)

#### Part B Workshop

* [Getting Started with Continuous Integration for MLOps](https://github.com/FourthBrain/databricks-zero-to-mlops/blob/main/docs/week1-notes.md#workshop-b-getting-started-with-continuous-integration)

#### Readings/Media

* [Quickstart Azure Databricks](https://docs.microsoft.com/en-us/azure/databricks/scenarios/quickstart-create-databricks-workspace-portal?tabs=azure-portal)

##### Create tables directly from imported data

* [Introduction to importing, reading, and modifying data](https://docs.microsoft.com/en-us/azure/databricks/data/data)
* [Databases and tables](https://docs.microsoft.com/en-us/azure/databricks/data/tables)
* [Metastores](https://docs.microsoft.com/en-us/azure/databricks/data/metastores/)

##### Ingest data into Azure Databricks

* [Databricks integrations](https://docs.microsoft.com/en-us/azure/databricks/integrations/)

##### Access data in Apache Spark formats and from external data sources

* [Data sources](https://docs.microsoft.com/en-us/azure/databricks/data/data-sources/)
* [Delta Lake guide](https://docs.microsoft.com/en-us/azure/databricks/delta/)

#### Labs

* [Github Actions pytest](https://github.com/noahgift/github-actions-pytest)
* [quickstart-create-databricks-workspace-portal](https://docs.microsoft.com/azure/azure-databricks/quickstart-create-databricks-workspace-portal)
* [Example databricks notebooks](https://github.com/FourthBrain/databricks-zero-to-mlops/tree/main/src/week1-getting-started)

#### Discussions

* Why is CI (Continuous Integration) a foundational component for MLOps?
* Why is logging, monitoring, and instrumentation so critical with distributed systems like Spark?
* What is the advantage of scheduling a notebook job in Databricks Spark?
* What are two ways to use data in Databricks Spark?

#### Assignments (Demo)

* Build out your own Github repository with a Python scaffold of:  `Makefile`, `requirements.txt`, a source file, and a test file and do:  `make lint && make test && make format`.
* Add a Jupyter Notebook to your Continuous Integration setup and test it with `pytest --nbval`. [nbval plugin reference](https://github.com/computationalmodelling/nbval). 
* Perform Exploratory Data Analysis with a Databricks Spark Cluster using the [Azure Open Datasets](https://docs.microsoft.com/en-us/azure/open-datasets/dataset-catalog). imported data or Databricks sample datasets. Please try both regular Pyspark as well as the new Pandas API.
* Schedule a notebook job to run nightly at midnight
* Create source code repository and integrate it with Databricks and build our a notebook in it you commit.

### Week Two:  Spark MLflow Tracking

#### Topics

* Topic:  Getting with ML & MLflow tracking
* Topic:  Getting started with containerizing Microservices

#### Learning Objectives

*   Compose Spark MLflow tracking solutions
*   Compose Containerized Microservice solutions

#### Part A Workshop

* [Getting with ML & MLflow tracking](https://github.com/FourthBrain/databricks-zero-to-mlops/blob/main/docs/week2-notes.md#workshop-a--getting-with-mlflow-tracking)

#### Part B Workshop
* [Getting started with containerizing Microservices](https://github.com/FourthBrain/databricks-zero-to-mlops/blob/main/docs/week2-notes.md#workshop-b-getting-started-with-containerizing-microservices)

#### Readings/Media

* [MLflow tracking](https://www.mlflow.org/docs/latest/tracking.html)
* [Databricks MLflow tracking](https://docs.databricks.com/applications/mlflow/tracking.html)
* [.NET 6 on AWS for Containers using Cloud9](https://github.com/noahgift/dot-net-6-aws)
* [Python MLOps Cookbook](https://github.com/noahgift/Python-MLOps-Cookbook)

#### Lab

#### Discussions

* How could experiment tracking increase productivity in a Data Science team?

#### Assignments (Demo)

* Using an Azure Open Dataset, perform several MLflow tracking experiments and identify the best runs.
* Deploy a containerized application to a Cloud Provider or Local Datacenter.

### Week Three: Spark MLflow Projects

#### Topics

* Topic: Getting started with ML & MLflow Projects
* Topic: Getting started with continuously deploying containerized Microservices
* Topic: Getting started with Kubernetes and Container Orchestration Solutions

#### Learning Objectives

*   Compose MLflow Projects solutions
*   Deploy Containerized Microservice solutions to a PaaS using Continuous Delivery
*   Compose Kubernetes Container Orchestration Solutions

#### Part A Workshop

#### Part B Workshop


#### Readings/Media

* [AWS App Runner Containerized Flask](https://github.com/noahgift/fastapi)

#### Lab

#### Discussions

* Why are containers an ideal mechanism for Continuous Delivery?

#### Assignments (Demo)

* Run an MLflow Project on Databricks using an Azure Open Dataset
* Deploy a containerized FastAPI microservice to AWS App Runner.  Alternatively, use a similar PaaS using Continuous Delivery via a Container Registry.

### Week Four: Spark MLflow Models and Model Registry

#### Topics

* Topic: Getting started with MLflow Models and the Model Registry
* Topic: Getting started with continuously deploying containerized Microservices

#### Learning Objectives

* Compose MLflow Model and Model Registry solutions
* Deploy a model from the Model Registry

#### Part A Workshop

#### Part B Workshop


#### Readings/Media

* [MLflow Models](https://www.mlflow.org/docs/latest/models.html)
* [MLflow Model Registry](https://www.mlflow.org/docs/latest/model-registry.html)

#### Lab

#### Discussions

* What are the advantages of versioning ML Models using the Model Registry?

#### Assignments (Demo)

* Evaluate a model with [`mlflow.evaluate`](https://www.mlflow.org/docs/latest/models.html#id20)
* Deploy a model using the model registry after [training on an Azure Open Dataset](https://www.mlflow.org/docs/latest/model-registry.html#serving-an-mlflow-model-from-model-registry)
