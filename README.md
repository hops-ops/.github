# hops: like in basketball, but for ops

hops is a cloud native gitops development platform, built from the ground up to be given away.

It is in very active development, and many of the repos that exist now are experimental.

The following are good!

## AWS Configurations

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

### AWS Helm Wrappers

| Name | Description | Repository |
|------|-------------|------------|
| cert-manager | cert-manager with AWS Pod Identity for Route53 DNS01 challenges | [hops-ops/helm-aws-cert-manager](https://github.com/hops-ops/helm-aws-cert-manager) |
| external-dns | external-dns with AWS Pod Identity for Route53 DNS record management | [hops-ops/helm-aws-external-dns](https://github.com/hops-ops/helm-aws-external-dns) |
| external-secrets | external-secrets with AWS Pod Identity for Secrets Manager and SSM Parameter Store | [hops-ops/helm-aws-external-secrets](https://github.com/hops-ops/helm-aws-external-secrets) |
| load-balancer-controller | AWS Load Balancer Controller with automated Pod Identity for IAM permissions | [hops-ops/helm-aws-load-balancer-controller](https://github.com/hops-ops/helm-aws-load-balancer-controller) |

### AWS Stacks

| Name | Description | Repository |
|------|-------------|------------|
| observe | Observe stack with AWS Pod Identity for OpenCost billing access, and s3 data stores. | [hops-ops/stack-aws-observe](https://github.com/hops-ops/stack-aws-observe) |

## Stacks

| Name | Description | Repository |
|------|-------------|------------|
| istio | Istio (base, istiod, gateways) with observability defaults and optional egress allowlisting | [hops-ops/stack-istio](https://github.com/hops-ops/stack-istio) |
| knative | Knative Serving, Eventing, and optional NATS JetStream on any cluster with Istio | [hops-ops/stack-knative](https://github.com/hops-ops/stack-knative) |
| observe | Complete observability stack -- metrics, logs, traces, cost monitoring, and Grafana dashboards | [hops-ops/stack-observe](https://github.com/hops-ops/stack-observe) |
