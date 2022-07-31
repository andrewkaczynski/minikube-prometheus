# MINIKUBE PROMETHEUS LAB

This is repository for the prometheus lab built on top of minikube with conjuction to Argo CD.

## Requirements

The lab has been tested on **UBUNTU 22.04 LTS**. The following tools are required to make it works:
* minikube >= v1.26.0
* helm >= 3.7.1
* task >= v3.14.0
* kubectl >= v1.24.1

## Installation

Repository contains **Taskfile.yml** with all the necessary tasks included. Make sure you have task cli installed, then execute:

```bash
task build
```

After couple of minutes the cluster will be up and running.


## Acess to ARGO CD web console

When *task build* will finish, it will print out the URL to your Argo CD dashboard. Use the following credentials:

```bash
admin:argocd
```