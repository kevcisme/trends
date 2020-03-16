FROM jupyter/pyspark-notebook

USER root
RUN sudo apt-get update && apt-get install -y \
  libpq-dev \
  vim

USER jovyan 
COPY ./requirements.txt /home/jovyan/requirements.txt
RUN pip install -r /home/jovyan/requirements.txt