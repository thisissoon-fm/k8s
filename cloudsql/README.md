# Cloud SQL

A Cloud SQL Proxy is required to allow Kubernetes to talk to Cloud SQL
hosted databases.

The crednetials should already be created in Cloud SQL and the Kubernetes cluster.

If not please follow the guide here: https://cloud.google.com/sql/docs/postgres/connect-container-engine

## Create Replication Controller and Service

```
kubectl create -f ./cloudsql/controller.yml
```

```
kubectl create -f ./cloudsql/service.yml
```
