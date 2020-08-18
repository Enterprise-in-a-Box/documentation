# Enterprise in a Box (EIAB)


This is an effort to describe and deliver user interfaces, enterprise tooling, and integration patterns. Opinions on how to build your software are excluded, and a solid understanding of enterprise integration solutions are more valued.

# Goals / Approach - Backing services

Scaling, provisioning, instrumentation, and administration of services are brought under a unified and open source platform as a service.

- GraphQL fragment/stitching with routing to internal RESTful services
- A set of common enterprise integration patterns as a service (Messages, Observers, Queues, Routes, ETL)
- A Kuberetes cluster of FastAPI microservices
- A Postgres SQL Server for persistence
- A serverless approach to pre-rendering/caching of the UI
- Robust admin tool to create, monitor, and deploy application services

## Buisness Objects

Each FastAPI microservice stewards over a single instance of a business object. Let's use Cars for example. A car has properties like wheels, color, created date, etc. EIAB lets an adminstrator create models and define their attributes. Attributes can have concerns attached to enable relationships, observers, etc.

## Integration services

EIAB aims to make building integration patterns a matter of drag and drop. Concerns are designed in the administrative console and then attached to the attributes that need effected.


# Goals / Approach - Frontend services

EIAB aims to drive consumer facing applications through a well defined JSON schema of components, concerns, attributes, and values. A component library and scaffolding tool allows product owners to quickly build functioning prototypes backed by real data.
