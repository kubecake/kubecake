# Minikube tutorial

## Lesson 0: Intro to Kubernetes

Requisites:

* Docker
* Docker Hub account
* Kubectl
* Minikube

In [simple](./simple/index.md) you will find how to build a Docker image for an Apache+php app, run it locally with Docker and upload it to Docker Hub.
Then, you will deploy it on a Minikube local cluster, using a deployment and service definition.

In [stateful](./stateful/index.md) you will deploy an stateful WordPress installation, with a pod for PHP files and another one for MySQL databases that uses a PersistantVolumeClaim to have a persistant database.