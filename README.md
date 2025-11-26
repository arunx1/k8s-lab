## Practice User management project.
### Backend Services:
- Java Spring Boot
- Python FastApi

### Frontend:
- Vite + Tailwind + VueJS + TS

### Database:
- Postgres

### Distributed caching:
- Redis

### Infra
- MicroK8s on multipass
- Docker with local image registry

### Setup:
<img width="802" height="732" alt="Screenshot 2025-11-26 at 2 47 21 PM" src="https://github.com/user-attachments/assets/8f76f42a-f712-4702-b697-2b4945edf5df" />

### Project overview
https://github.com/user-attachments/assets/644ddcaa-9065-4dd7-9d55-e5cdec685ca7

### Test Report 
- Running both java and python api's with 20 threads distributed on creating new users, fetching existing user through java api, fetching existing user through python api.
- User list always returned from postgres
- individual user first checked in redis, if cache miss, fetched from postgres and cached in redis. Next hit on same user id would serve from redis.
  
