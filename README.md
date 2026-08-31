# configuration-repo

Git repository consumed by Spring Cloud Config Server.

## Files
- `application.yml` - shared defaults
- `customer-service.yml` - customer configuration
- `account-service.yml` - account configuration
- `transaction-service.yml` - transaction configuration
- `api-gateway.yml` - gateway routes + local service instances

## Production direction
In AWS/EKS, replace local service instance URIs with Kubernetes service discovery rather than keeping localhost addresses.
Sensitive values will move to AWS Secrets Manager in a later milestone.
