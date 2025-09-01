# MSA Demo Project

Spring Boot + Spring Cloud 기반의 MSA 전환 데모 프로젝트입니다.  
API Gateway, Service Discovery, Message Queue, JWT 인증 등을 포함합니다.

## 📌 아키텍처
```mermaid
graph TD
  Client --> Gateway --> UserService
  Gateway --> OrderService --> PaymentService
  OrderService -->|Event| Kafka --> PaymentService
