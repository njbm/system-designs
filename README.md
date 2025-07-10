# 📐 System Designs

A collection of high-level system architecture notes and diagrams for real-world scalable applications.

---

## 🔹 E-Commerce Platform

**Components:**

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


🔹 Real-Time Chat App
Components:

Frontend (React / Vue + WebSocket)

WebSocket server (Laravel Echo + Redis)

User presence tracking

Message delivery queues

Typing indicator, read receipts

MongoDB + Redis