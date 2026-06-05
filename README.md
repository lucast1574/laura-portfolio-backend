# Laura Portfolio Backend

NestJS + GraphQL + MongoDB. Igual al backend del portfolio de Lucas — solo cambia el nombre del package, el dominio (`backend.santillan.pro`) y el SiteConfig por defecto (Laura, Data Engineer).

## Endpoints
- `POST /graphql` — GraphQL API
- `GET /health` — Health check
- Playground en dev en `/graphql`

## Variables
Ver `.env.example`.

## Seed admin user
```bash
SEED_USERNAME=laura SEED_PASSWORD='***' npm run seed
```

O via mutation one-shot:
```graphql
mutation { bootstrapAdmin(username: "laura", password: "...", secret: "BOOTSTRAP_SECRET") }
```
