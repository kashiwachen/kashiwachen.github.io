# Multi-tenant DB

Everyone is always talking about developing a SaaS app. The basis for SaaS is a Multi-tenancy architecture that allows multiple tenants (organizations) access to multiple instances of the software hosted on a single server. The tenants of the software share the server resources and memory.

Designing a database structure that can accommodate this type of design depends on several factors among them:

● Security

● Client data isolation

● Database scalability

● Database management (backup and restoration)

● Operational complexities such as schema and tenant management

● Speed

## Ways to design DB

There are a few different ways to design your database depending on your requirements Ill explain those below.

1. Database-per-tenant
2. Multi-tenant database
3. Single multi-tenant database
4. Sharded multi-tenant database

# TODO:

- [ ] Get the abstract from [article](https://blakebhowe.medium.com/multi-tenant-application-database-design-e4c2d161f3dd)