# Koa Bark

An es7 friendly framework for NodeJS applications.  

The framework is built on top of
- Koa 2
- Sequelize
- Socket.io

Install all dependencies
```
npm install
```

The app requires a postgres database (current hard coded to localhost port 5432).
Create a '.env' file in the project's root folder with the following information:  
```
username=yourpostgresusername
password=yourpostgrespassword
dbname=yourdbname
PORT=whatverportyouwant
```

Run server  
```
npm start
```


Run tests  
```
npm test
```


## Middleware
The goal of the middleware is to follow an MVC pattern.  
- Model: Declare in the model folder any database items or relationships  
- View: Create any UI or client js in the client folder  
- Controller: Write all routing logic in the server folder  
- Test: Write all server tests in the test/test.js file  

For the to-do list example, all documentation follows a Swagger yaml definition  
Ideally, in the future the swagger definition should drive a set of tests as well  
The documentation is available at '<endpoint>/docs', in this case, they're at localhost:<port>/docs
