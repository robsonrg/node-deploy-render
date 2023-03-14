# Deploy Node app on Render

Based on video https://www.youtube.com/watch?v=pmXfvd6Zqg4, I create this repo for test and deploy an node app on [Render](https://render.com/).

Using:

- `typescript`
- `prisma` for ORM
- `tsup` for build
- `fastify` for simple routes
- `zod` for data validations

And use `postgresql` for database.

---

## Install and run locally

1 - Install node modules
```sh
$ npm install
```

2 - Config postgresql string connection on `.env` file

3 - Start postgresql container
```sh
$ docker compose up -d
```

4 - Install migrations
```sh
$ npx prisma migrate dev
```

5 - Start HTTP Server
```sh
$ npm run dev
```

Now, you can list users: http://localhost:3333/users