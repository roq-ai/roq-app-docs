#### Prerequisites
Node.js, Next.js
#### Setup your environment variables
```bash
cp .env.example .env
# Add your environment variables from the console. Use the "Copy env" button
```

#### Startup your database
**Option 1:** You can run any database that is supported by [PrismaORM](https://www.prisma.io/)

**Option 2:** Or you can install Postgres by using Docker. Make sure no other Postgres instance is running on the same machine.
```bash
docker-compose up
```
For both options, add the database connection string to your `.env` file:
```dotenv
DATABASE_URL=postgres://yourusername:yourpassword@localhost:5432/yourdb
```

#### Install dependencies and start up your app
```bash
npm install #or yarn
npm run dev #or yarn dev
```
Now you can open your app at [http://localhost:3000](http://localhost:3000).
