# Airflow Celery Workers

<p>
<img alt="Docker" src="https://img.shields.io/badge/docker-%230db7ed.svg?&style=for-the-badge&logo=docker&logoColor=white"/>
<img alt="Apache Airflow" src="https://img.shields.io/badge/apacheairflow-%23017cee.svg?&style=for-the-badge&logo=apache-airflow&logoColor=white"/>
<img alt="Celery" src="https://img.shields.io/badge/celery-%2337814A.svg?&style=for-the-badge&logo=celery&logoColor=white"/>
<img alt="Redis" src="https://img.shields.io/badge/redis-%23DC382D.svg?&style=for-the-badge&logo=redis&logoColor=white"/>
</p>

This repo contains a setup to config Airflow 2.0 with Celery workers. To do it, two databases (Postgres and Redis) are setup: a Postgres container to serve as a metadatabase; and Redis as the broker database and connection between the scheduler and workers. Besides the two database and worker containers, the scheduler and other two UIs are also setup with docker: Airflow Webserver (by default, at port 8080) and Airflow Celery Flower (by default, at port 5555). The following diagram represents the infrasctructure builded:

<p align="center"><img src="./img/diagram.jpg"></p>