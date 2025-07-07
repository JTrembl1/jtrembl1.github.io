mermaid
```
graph TB
    subgraph "Client Layer"
        A[Web Portal]
        B[Mobile App]
        C[Third-party Integrations]
    end
    
    subgraph "API Gateway Layer"
        D[APIM Gateway]
        E[OAuth2 Authentication]
        F[Rate Limiting]
    end
    
    subgraph "Business Logic Layer"
        G[Logic Apps Workflows]
        H[Azure Functions]
        I[Service Bus]
    end
    
    subgraph "Data Layer"
        J[NCF SQL Database]
        K[GraphQL API]
        L[REN/iPhiCore System]
    end
    
    A --> D
    B --> D
    C --> D
    D --> G
    D --> H
    G --> I
    H --> I
    I --> J
    I --> K
    I --> L
```
