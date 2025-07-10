# 🛒 E-Commerce Platform System Design

## Components
- Web frontend (Next.js / Vue.js)
- Backend (Laravel REST API)
- Payment Gateway (Stripe/SSLCommerz)
- Product catalog service
- Order & inventory service
- Notification service (email/SMS)
- MySQL + Redis + S3 (AWS)

```mermaid
graph TD
  A[Client App] --> B[API Gateway]
  B --> C[Auth Service]
  B --> D[Product Service]
  B --> E[Order Service]
  E --> F[Payment Gateway]
  E --> G[Inventory Service]
  B --> H[Notification Service]
  D --> I[(MySQL)]
  G --> J[(Redis Cache)]
  H --> K[(Mail/SMS Queue)]
```
