## Sample for authentication use json web tokken

## I. Build Backend
- Create roles, user_roles, users table in first starting
- Change in server.js (enable below code) 
- Enter Postgre env infomation in /node-js-jwt-auth/app/config/db.config.js

```
//force: true will drop the table if it already exists
db.sequelize.sync({force: true}).then(() => {
  console.log('Drop and Resync Database with { force: true }');
  initial();
});
```
- Build backend
```
cd node-js-jwt-auth/
npm install
node server.js
```

## II. Build Frontend
```
cd react-hooks-jwt-auth/
yarn
yarn start
```