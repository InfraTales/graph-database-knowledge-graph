# Security Overview

Security posture of **Knowledge Graph**.

## Data Protection

- **Encryption at rest**: KMS encryption
- **Encryption in transit**: TLS required
- **VPC isolation**: Private subnets only
- **IAM authentication**: Database access

## Access Controls

- **IAM policies**: Fine-grained access
- **Security groups**: Network isolation
- **Audit logging**: CloudTrail integration
- **Query logging**: Neptune slow query logs

## Graph-Specific Security

- **Traversal limits**: Prevent expensive queries
- **Property access**: Control sensitive attributes
- **Relationship filtering**: Limit visible edges

## Compliance

- SOC 2 Type II
- GDPR (with data controls)
- PCI-DSS (with encryption)

> See `SECURITY.md` for detailed configurations.
