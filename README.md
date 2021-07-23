# Analysis of Jupyterhub application pods in the Operate First Enviornment

This repository contains a set of obfuscated sample datasets, as well as example analysis notebooks that can be used to quickly get started exploring and interacting with the Operate First Jupyterhub's operations data. We are also working on updating the notebooks to make it easy for users to pull additional data themselves.

The data provided (at the moment) contains **metrics**, **logs**, and **events** records from the Jupyterhub application on the [operate first cluster](https://www.operate-first.cloud/) on the Massachusetts Open Cloud (MOC). This is an Open Cloud environment, with reproducibility built-in, operated by a community with the goal of operating software in a production-grade environment.
<br><br>


## DATASETS

### METRICS

The metrics dataset consists of five seperate timeseries, each broken into their own csv file. Each metric contains around 1 days worth of data sampled every few minutes.

* [Notebook](/notebooks/jupyterhub_data.ipynb)
* [Data](/data/processed/jupyterhub/metrics)
* [Source](http://thanos-query-frontend-opf-observatorium.apps.zero.massopen.cloud/)

### LOGS

The logs dataset includes roughly 1 day of infrastructure logs stored as a single json.

* [Notebook](/notebooks/jupyterhub_data.ipynb)
* [Data](/data/processed/jupyterhub/logs)
* [Source](https://elasticsearch-openshift-logging.apps.zero.massopen.cloud/)

### Events

The events dataset was collected by a cluster admin and contains cluster wide events for Jupyterhub application for a day.

* [Notebook](notebooks/jupyterhub_data.ipynb)
* [Data](/data/processed/jupyterhub/events)
* [Source](https://console-openshift-console.apps.zero.massopen.cloud/)
