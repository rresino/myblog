---
layout: post
title: Kubernetes - Pods - Snippets
date:   2021-04-22 12:00:00 +0200
categories: [k8s, pod]
---

It's my personal compilation of quick snippets for Kubernetes and Pods.

## Get all pods

```bash
kubectl get pods
```

## Get all info and details of a pod

```bash
kubectl describe pod <pod name>
```

## How to connect to one pod

```bash
kubectl exec -it <pod name> /bin/bash
kubectl exec -it <pod name> -- /bin/bash
```

## Copy file inside a pod

```bash
kubectl cp <file to copy> <pod name>:<path to copy file inside pod>
```

## See logs of one pod

```bash
kubectl logs <name of pod> -f --timestamps
```

## How to see the pods how consume more resources

```bash
kubectl top pods
```
