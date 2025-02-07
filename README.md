# nestjs-mysql-prisma-dev-container-example

1. Reopen in Dev Container


2. In a dev container
```
npm i
npx prisma migrate dev
npm run start:dev
```

3. call api

```
curl --location 'http://localhost:3000/user' \
--header 'Content-Type: application/json' \
--data-raw '{
    "name":"User1",
    "email":"user1@example.com"
}'
```

```
curl --location 'http://localhost:3000/post' \
--header 'Content-Type: application/json' \
--data-raw '{
    "title":"Post-title",
    "content":"Post-content",
    "authorEmail":"user1@example.com"
}'
```