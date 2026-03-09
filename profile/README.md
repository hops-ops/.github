# hops: like in basketball, but for ops

hops is a cloud native gitops development platform, built from the ground up to be given away.

It is in very active development, and many of the repos that exist now are experimental.

The following are good!

## AWS

### Configurations

| Name | Description | Repository |
|------|-------------|------------|
| account | Create and manage AWS Organizations member accounts | [hops-ops/aws-account](https://github.com/hops-ops/aws-account) |
| actions-connector | GitHub Actions OIDC federation with AWS for secure CI/CD | [hops-ops/aws-actions-connector](https://github.com/hops-ops/aws-actions-connector) |
| auto-eks-cluster | Production-ready EKS clusters with Auto Mode enabled | [hops-ops/aws-auto-eks-cluster](https://github.com/hops-ops/aws-auto-eks-cluster) |
| foundation | Single resource for your entire AWS foundation -- Organization, Identity Center, IPAM, and Network | [hops-ops/aws-foundation](https://github.com/hops-ops/aws-foundation) |
| identity-center | Manage AWS IAM Identity Center (SSO) -- groups, users, permission sets, and account assignments | [hops-ops/aws-identity-center](https://github.com/hops-ops/aws-identity-center) |
| irsa | You should probably use pod-identity instead of this, but if you need it, IAM Roles for Service Accounts so Kubernetes workloads can assume AWS roles | [hops-ops/aws-irsa](https://github.com/hops-ops/aws-irsa) |
| network | Production-ready VPCs with IPAM-backed CIDR allocation and dual-stack IPv6 support | [hops-ops/aws-network](https://github.com/hops-ops/aws-network) |
| organization | Manage your AWS Organization, OUs, and Accounts as a single resource | [hops-ops/aws-organization](https://github.com/hops-ops/aws-organization) |
| pod-identity | IAM roles and EKS Pod Identity associations for Kubernetes service accounts | [hops-ops/aws-pod-identity](https://github.com/hops-ops/aws-pod-identity) |
| ram-share | Share AWS resources across accounts using Resource Access Manager | [hops-ops/aws-ram-share](https://github.com/hops-ops/aws-ram-share) |

### Stacks

| Name | Description | Repository |
|------|-------------|------------|
| base | Base stack for AWS. Includes `aws-load-balancer-controller`. | [hops-ops/aws-base-stack](https://github.com/hops-ops/aws-base-stack) |
| crossplane | Crossplane stack for AWS. Installs and configures Crossplane and aws, github, helm, and k8s, providers.  | [hops-ops/aws-crossplane-stack](https://github.com/hops-ops/aws-crossplane-stack) |
| dns | DNS stack for AWS.  | [hops-ops/aws-dns-stack](https://github.com/hops-ops/aws-dns-stack) |
| observe | Observe stack with Prometheus for Metrics, Alertmanager for Alerts, Loki for logs, Grafana + Operator + Datasources + Dashboards, Tempo for tracing data, k8s-monitoring chart for Alloy, and OpenCost for cost reporting. | [hops-ops/aws-observe-stack](https://github.com/hops-ops/aws-observe-stack) |
| secret | Secret stack – External Secrets plus ClusterStore config connected to AWS Secrets Manager | [hops-ops/aws-secret-stack](https://github.com/hops-ops/aws-secret-stack) |

## Platform Agnostic

### Helm Charts

| Name | Description | Repository |
|------|-------------|------------|
| metrics-server | Kubernetes Metrics Server for HPA, VPA, and kubectl top | [hops-ops/helm-metrics-server](https://github.com/hops-ops/helm-metrics-server) |

### Stacks

| Name | Description | Repository |
|------|-------------|------------|
| istio | Istio (base, istiod, gateways) with observability defaults and optional egress allowlisting | [hops-ops/stack-istio](https://github.com/hops-ops/stack-istio) |
| knative | Knative Serving, Eventing, and optional NATS JetStream on any cluster with Istio | [hops-ops/stack-knative](https://github.com/hops-ops/stack-knative) |
| observe | Complete observability stack -- metrics, logs, traces, cost monitoring, and Grafana dashboards | [hops-ops/stack-observe](https://github.com/hops-ops/stack-observe) |
