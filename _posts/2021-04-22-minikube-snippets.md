---
layout: post
title: Kubernetes - Minikube - Snippets
date:   2021-04-22 16:00:00 +0200
categories: [k8s, minikube]
---

## Start a new minikube cluster and set manually the k8s version

```bash
minikube start --kubernetes-version <k8s version>
```

## Run K8S dashboard

```bash
minikube dashboard
```

## Get url from K8S service

```bash
minikube service <service name> --url --namespace <namespace name>
```

## Drop current cluster

```bash
minikube delete
```

## Enable load balancer for minikube 

```bash
minikube tunnel
```

If minikube don't clean the tunnel network, you can force the clean up using:

```bash
minikube tunnel --cleanup
```

## Get minikube cluster ip

```bash
minikube ip
minikube ip -n minikube
```
