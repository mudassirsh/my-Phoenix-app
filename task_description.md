# Task Description

DevOps Code Challenge for Backgammon Galaxy

## Goal

We need to develop a GitOps Platform to manage our applications which run in Kubernetes.

Use this repository to create a GitOps approach for managing your local kubernetes environment (kind, minikube,...).

The source code of our application can be found [here](https://github.com/nickjj/docker-phoenix-example). As database, it needs PostgreSQL, install [CloudNativePG](https://cloudnative-pg.io/) (Helm Charts). As we need some metrics from the DB, install [prometheus](https://github.com/prometheus-community/helm-charts/blob/main/charts/kube-prometheus-stack) and look for a good Grafana Dashboard for CloudNativePG.

There is no Helm Chart for our application, so you need to build one.

Open a PR against git main branch of this repository.

## Technologies

* Kubernetes
* Flux
* Helm
* Kustomize
* Docker
* Prometheus
* Grafana
* Postgres

## Configuration

We can set up the app through environment variables (check [runtime.exs](https://github.com/nickjj/docker-phoenix-example/blob/main/config/runtime.exs)) but from operations perspective, everything should be managed using helm chart configurations.

## Repositories

Use docker hub for storing the docker image of the application and this git repository to store the app helm chart.

## Docs

Add the necessary documentation to [README.md](README.md)

## Bonus

Send alarm/notification when the pods are failing (You can use whatever platform: slack, email, ...)
