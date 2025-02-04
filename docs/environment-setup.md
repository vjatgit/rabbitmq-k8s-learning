# Complete Environment Setup Guide

## 1. Install Homebrew (Package Manager)
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## 2. Install Required Tools

### Install Minikube
```bash
brew install minikube
```

### Install kubectl
```bash
brew install kubectl
```

### Install Helm
```bash
brew install helm
```

## 3. Start Minikube
```bash
# Start with recommended resources for RabbitMQ
minikube start --cpus 2 --memory 4096
```

## 4. Verify Installation
```bash
# Check Minikube status
minikube status

# Check kubectl
kubectl version --client

# Check Helm
helm version
```

## System Requirements
- macOS 10.13 or newer
- 2 CPU cores
- 4GB RAM minimum (8GB recommended)
- 20GB free disk space
- Internet connection

## Next Steps After Installation
1. Start Minikube cluster
2. Deploy test application
3. Access Kubernetes dashboard
4. Begin RabbitMQ deployment

## Troubleshooting

### Common Issues
1. **Not Enough Resources**
   - Close unnecessary applications
   - Increase Minikube resource allocation

2. **Network Issues**
   - Check internet connection
   - Verify VPN settings

3. **Permission Issues**
   - Run with sudo if needed
   - Check file permissions
