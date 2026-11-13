# vProfile on Kubernetes – Manifests

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white) ![Tomcat](https://img.shields.io/badge/Tomcat-F8DC75?logo=apachetomcat&logoColor=black) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![Memcached](https://img.shields.io/badge/Memcached-2C5BB4) ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?logo=rabbitmq&logoColor=white)

> Kubernetes manifests to run the multi-tier vProfile stack: app, MySQL, Memcached and RabbitMQ.

## Overview

Kubernetes manifests that run the **vProfile** multi-tier stack: the Tomcat application, a **MySQL** database, **Memcached** and **RabbitMQ**, each with its own Deployment and internal ClusterIP Service, plus an externally exposed app Service and a Secret for the database and broker passwords.

## Tech Stack

- **Kubernetes**
- **Tomcat**
- **MySQL**
- **Memcached**
- **RabbitMQ**

## Repository Structure

```text
app-db-dep.yml
app-dep.yml
app-secret.yml
app-service.yml
db-cip.yml
mc-cip.yml
mc-dep.yml
README.md
rmq-cip.yml
rmq-dep.yml
```

## Getting Started

```bash
kubectl apply -f .
kubectl get pods,svc
```

## Author

**Gamal Mohammad**

[![GitHub](https://img.shields.io/badge/GitHub-Gamal--Mohammad-181717?logo=github)](https://github.com/Gamal-Mohammad)
