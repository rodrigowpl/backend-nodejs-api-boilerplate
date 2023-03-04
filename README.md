# Boilerplate API

## Engineering

### Tech stack
- [Node](https://github.com/nodejs/node)
- [Express](https://github.com/expressjs/express)
- [GraphQL](https://github.com/graphql/graphql-js)
- [Apollo Server](https://github.com/apollographql/apollo-server)
- [Typescript](https://www.typescriptlang.org/)
- [Prisma](https://www.prisma.io/)

## Dependencies
- Node js => v16
- Yarn or Npm

## Up and Running
- Install dependencies `yarn`
- Run `yarn dev` to run development server (will be available in `http://localhost:9001` and GraphQL in `http://localhost:9001/graphql`)
- Create `.env` file based on `.env.example`
- Run `npx prisma migrate dev` to generate your database
  - **`Important`**: **Run this command for local database only. Do not ever run this on production**. If you are using a shared developer database on cloud. Talk to your teammates before to run this command -- it might not be needed.
  - [See Prisma Migrate](https://www.prisma.io/docs/concepts/components/prisma-migrate) for more detail

## Useful tip
- Run `npx prisma studio` to have a bult-in database client

## Available scripts
- `yarn start (or npm start)`: Run server in production mode
- `yarn dev (or npm dev)`: Run server in development mode
- `yarn build (or npm run build)`: Generate production build (files will be available on `build` directory)
- `yarn lint (or npm run lint)`: Run linter based on eslint configurations
- `yarn lint:fix (or npm run lint:fix )`: Run linter and fix errors
