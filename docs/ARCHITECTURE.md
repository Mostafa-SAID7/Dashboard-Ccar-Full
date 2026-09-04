# Architecture Overview

## Backend Architecture (Clean Architecture)

### Layers

1. **WebAPI** - REST API endpoints and controllers
2. **Application** - Business logic and use cases
3. **Domain** - Core business entities and rules
4. **Infrastructure** - External services and data access
5. **Persistence** - Database context and repositories

### Pattern: Clean Architecture
- Independent of frameworks
- Testable
- UI independent
- Database independent
- Framework independent

## Frontend Architecture (Angular)

### Structure

- **Components** - Reusable UI components
- **Services** - API communication and business logic
- **Guards** - Route protection and authorization
- **Interceptors** - HTTP request/response handling
- **Models** - TypeScript interfaces and types

## Communication Flow

```
Frontend (Angular) <--> Backend API (.NET) <--> Database (SQL Server)
```

## Database

- **Type**: SQL Server
- **ORM**: Entity Framework Core
- **Migrations**: Code-first approach
