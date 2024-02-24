Sight. A practice project that is small clone of Twitch and is built to make streaming web app with livekit
and has been followed by a tutorial and some part of this code if different such as database

> [!NOTE]
> the database in this project is Localized but remote dbs are functional.

![database ERD.](/public/postgresql-local-db.png)
* Data base ERD

### Prerequisites

**Node version 18.17 or later**

### Install packages

```shell
npm i
```

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/
CLERK_WEBHOOK_SECRET=

DATABASE_URL=

LIVEKIT_API_URL=
LIVEKIT_API_KEY=
LIVEKIT_API_SECRET=
NEXT_PUBLIC_LIVEKIT_WS_URL=

UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=
```

### Setup Prisma

Add Postgresql

```shell
npx prisma generate
npx prisma db push

```

### Start the app

```shell
npm run dev
```
