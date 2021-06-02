** Airflow **

This is for setting up a Docker-based Airflow
Download the files locally and run the following set of commands

1. docker build --tag airflow .
2. docker run --name my_airflow -it -d -p 8080:8080 airflow
3. docker ps
4. Check logs: docker logs my_airflow

***Issues***

1. Warnings show up as you are running pip as a root. Haven't resolved it.
2. Warnings on missing apt-utils can be ignored.
3. Hardwired for Aitflow 1.10.14! You need to edit the files to advance versions (including constraints file URL in Dockerfile)



