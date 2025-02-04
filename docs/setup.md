# Local Development Environment Setup

## Prerequisites Installation

### 1. Install Minikube
```bash
# Using Homebrew
brew install minikube

# Start Minikube with enough resources for RabbitMQ
minikube start --cpus 2 --memory 4096
```

### 2. Install kubectl (if not installed)
```bash
brew install kubectl
```

### 3. Install Helm (for RabbitMQ Operator)
```bash
brew install helm
```

### 4. Verify Installation
```bash
# Check Minikube
minikube status

# Check kubectl
kubectl version --client

# Check Helm
helm version
```

## RabbitMQ Operator Setup

### 1. Add RabbitMQ Helm Repository
```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update
```

### 2. Create Namespace
```bash
kubectl create namespace rabbitmq-system
```

### 3. Install RabbitMQ Operator
```bash
helm install rabbitmq-operator bitnami/rabbitmq-cluster-operator \
  --namespace rabbitmq-system
```

## Verification Steps

### 1. Check Operator Status
```bash
kubectl get pods -n rabbitmq-system
```

### 2. Create Test RabbitMQ Instance
```bash
# We'll create this in our next session
```

## Next Steps
1. Set up monitoring tools
2. Configure persistent storage
3. Deploy sample application

## Troubleshooting

### Common Issues
1. Insufficient Resources
   - Increase Minikube memory/CPU
   - Clean up unused resources

2. Network Issues
   - Check Minikube network
   - Verify port forwarding

3. Permission Issues
   - Verify RBAC settings
   - Check namespace permissions
