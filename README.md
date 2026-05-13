# Full-stack Express + Prisma + PostgreSQL Template

## 1. Create repo from template

Click “Use this template” on GitHub and create your new repository.

## 2. Install dependencies

`npm install`

## 3. Create PostgreSQL database

Open PostgreSQL shell:  
`psql`

Create database:  
`CREATE DATABASE mydatabase;`

Exit psql:  
`\q`

## 4. Create `.env` file (project root)

Similar to:

```
DATABASE_URL="postgresql://username:password@localhost:5432/mydatabase"
COOKIE_SECRET="secret_cookie"
```

## 5. Run Prisma migrations

`npx prisma migrate dev --name init`

## 6. Generate Prisma client

`npx prisma generate`

## 7. Update app configuration

In `app.js`, set your app title:  
`res.locals.appTitle = "appTitleGoesHere";`

## 8. Update package metadata

In `package.json`, update any placeholder with "express-prisma-psql-template" to the new repo name

## 9. Update README

Replace this README with project-specific documentation.

## 10. Start development server

`npm run dev`
