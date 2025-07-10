# 💸 Online Payment System Design

## Components
- User Wallet Service
- Transaction Ledger
- Fraud Detection Microservice
- Currency Exchange (optional)
- Admin Dashboard
- MySQL, Kafka, Redis, Cloud Logs

```mermaid
graph TD
  A[User App] --> B[Wallet Service]
  B --> C[Ledger DB]
  B --> D[Exchange Service]
  B --> E[Fraud Detection]
  E --> F[Risk Flags DB]
  B --> G[Kafka Stream for Auditing]
  G --> H[Log Storage]
  Admin --> I[Dashboard Service] --> B
```
