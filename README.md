# ai-monitoring-redis

Redis for API Gateway rate limiting. Deploys via Bitnami Helm chart.

Default branch: **develop**.

## Prerequisite

`ai-monitoring-secrets` must exist. Run **ai-monitoring-postgresql** first.

## Quick start

```bash
./deployments/install.sh
```

## Deploy via PR comment.

`/deploy aks`, `/deploy openshift`, or `/deploy oc` (same as OpenShift) on any PR.

## Required GitHub secrets

- **AKS:** AZURE_CREDENTIALS, AKS_RESOURCE_GROUP, AKS_CLUSTER_NAME
- **OpenShift:** OPENSHIFT_TOKEN, OPENSHIFT_SERVER, OPENSHIFT_PROJECT
- **Both:** DB_PASSWORD, JWT_SECRET
- **Optional:** REDIS_PASSWORD, RABBITMQ_PASSWORD (default to DB_PASSWORD)
