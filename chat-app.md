# 💬 Real-Time Chat App Design

## Components
- Frontend (React / Vue + WebSocket)
- WebSocket server (Laravel Echo + Redis)
- User presence tracking
- Message delivery queues
- Typing indicator, read receipts
- MongoDB + Redis

```mermaid
graph TD
  A[User Client] --> B[WebSocket Server]
  B --> C[Message Queue]
  B --> D[Presence Tracker]
  C --> E[(MongoDB)]
  D --> F[(Redis)]
```
