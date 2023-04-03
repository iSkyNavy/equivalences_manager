# Strapi Mysql Starter

Just a 2022 template ready to use with:

- strapi V4
- mysql


# Requirements
- Nodejs ≥ 16
- Mysql database. You could use this docker snippet https://gist.github.com/jrichardsz/73142c5c7eb7136d80b165e75d3a1e22

# Start strapi

- Create a database inside mysql instance with name is "equivalences_manager"
- Export or configure this environment variables

```sh
export HOST=0.0.0.0
export PORT=1337
export APP_KEYS="toBeModified1,toBeModified2"
export API_TOKEN_SALT=tobemodified
export ADMIN_JWT_SECRET=tobemodified
export JWT_SECRET=tobemodified
```

> Configure this variables in heroku web panel

- Excute:

```sh
npm install
npm run start
```

# Start strapi with docker

## Steps

```
- create .env file and copy content of .env.example and put values
- docker-compose up --build
```

## Use API - Steps


- create user
- get the jwt of user, consult htpp://yoururl/api/auth/local and send into body { identifier, password }, more information [get jwt user](https://docs.strapi.io/dev-docs/plugins/users-permissions)


<br>
> For more rest points, more detail on the wiki