# Runbook

## Deployment

```bash
terraform init && terraform apply -var="environment=prod"
```

## Loading Data

```bash
# Bulk load from S3
curl -X POST https://neptune:8182/loader \
  -d '{"source": "s3://bucket/data/", "format": "csv"}'
```

## Query Examples

```gremlin
// Find connected entities
g.V().has('type', 'person').out('knows').limit(10)

// Fraud detection pattern
g.V().has('account').as('a')
  .out('transaction').in('transaction')
  .where(neq('a')).dedup()
```

## Maintenance

- Monitor query latency daily
- Review slow query logs weekly
- Optimize indices monthly
- Test failover quarterly
