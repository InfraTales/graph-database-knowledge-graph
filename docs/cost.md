# Cost Analysis (₹)

Cost estimates for **Knowledge Graph** in **Indian Rupees (₹)**.

## Production Environment

| Service | Monthly Cost (₹) | Notes |
|---------|------------------|-------|
| **Neptune** | ₹80,000–150,000 | db.r5.large or larger |
| **Neptune Storage** | ₹10,000–30,000 | Per GB stored |
| **Neptune I/O** | ₹15,000–40,000 | Read/write requests |
| **Lambda** | ₹5,000–10,000 | Graph queries |
| **API Gateway** | ₹3,000–8,000 | Query API |
| **Total** | **₹115,000–240,000** | ~$1,440–3,000/month |

## Scaling Costs

| Cluster Size | Monthly Cost (₹) |
|-------------|------------------|
| 1 reader | ₹80,000–120,000 |
| 2 readers | ₹160,000–240,000 |
| 4 readers | ₹320,000–480,000 |

## Cost Optimization

- **Right-size instance** – Match to query patterns
- **Read replicas** – Scale reads separately
- **Query optimization** – Efficient Gremlin/SPARQL
- **Serverless** – Consider Neptune Serverless
