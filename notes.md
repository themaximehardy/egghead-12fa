# Notes

Launch MongoDB via Docker

```
docker volume create mongodbdata
```

```
docker run --name mongo -p 27017:27017 -v mongodbdata:/data/db -d mongo:latest
```

Create a `.env` file and add the environment variable: `MONGO_URI=mongodb://localhost:27017/foo`
Then use it in the file via `dotenv`. First `yarn add dotenv` and then `require('dotenv').config();`
You can use it like this: `process.env.MONGO_URI`.