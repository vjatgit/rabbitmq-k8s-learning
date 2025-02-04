# RabbitMQ on Kubernetes Learning Project

A hands-on project for learning RabbitMQ deployment and management on Kubernetes.

## Project Structure
```
├── kubernetes/           # K8s manifests
│   ├── base/            # Base configurations
│   └── overlays/        # Environment-specific configs
├── examples/            # Example applications
├── docs/               # Documentation
└── scripts/            # Utility scripts
```

## Learning Path

### Phase 1: Foundations (Week 1)
1. Local Development Setup
   - Minikube/Kind installation
   - Basic Kubernetes concepts
   - RabbitMQ basics

2. Single-node RabbitMQ
   - Basic deployment
   - Service exposure
   - Management interface

3. Simple Messaging
   - Basic publisher
   - Basic consumer
   - Queue management

### Phase 2: Clustering (Week 2)
1. RabbitMQ Cluster
   - Multi-node setup
   - Cluster configuration
   - High availability

2. StatefulSet Implementation
   - Persistent storage
   - Pod identity
   - Service discovery

3. Monitoring & Management
   - Prometheus metrics
   - Grafana dashboards
   - Health checks

### Phase 3: Production Ready (Week 3)
1. Security
   - TLS configuration
   - User management
   - Network policies

2. Backup & Recovery
   - Backup strategies
   - Restore procedures
   - Disaster recovery

3. Performance Tuning
   - Resource allocation
   - Queue optimization
   - Connection management

### Phase 4: Advanced Topics (Week 4)
1. Message Patterns
   - Pub/Sub
   - Request-Reply
   - Work Queues

2. Integration Patterns
   - Dead Letter Queues
   - Message TTL
   - Queue Federation

3. Production Deployment
   - CI/CD setup
   - Rolling updates
   - Blue-Green deployment

## Getting Started

### Prerequisites
1. Kubernetes cluster (Minikube/Kind)
2. kubectl CLI
3. Git
4. Basic understanding of messaging

### First Steps
1. Clone this repository
2. Set up local development environment
3. Follow the tutorials in docs/

## Documentation
- [Setup Guide](docs/setup.md)
- [Development Guide](docs/development.md)
- [Production Guide](docs/production.md)
- [Troubleshooting](docs/troubleshooting.md)

## Contributing
Feel free to contribute by:
1. Opening issues
2. Submitting pull requests
3. Improving documentation

## License
MIT
