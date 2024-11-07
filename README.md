# Mid Term lab Overview
---
This provides an overview of the mid-term lab.

## 1. Git Repository
- Initialized a repository
- **Main:** This branch is the code running in production.
- **Develop:** All the features ready to be tested and deployed
- **Feature/** 2 feature branches for cache-service and database-service.

## Services

---
These services are managed by Docker through Docker-Compose.yml which contains the environment that container needs to run and the sensitive info (password & username of postgreSQL) are stored in .env file (dummy data for now). 

.env file is also added to .gitignore to protect sensitive info.
---

- **Database Service**: PostgreSQL, exposed on port 5432.
- **Cache Service**: Redis, exposed on port 6379.

## Running the Services
To run both services using Docker Compose:
```sh
docker-compose up
