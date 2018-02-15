- set up file system based mvc framework
- create server.js
- create confing, controller,database,models,public,views folder
- config: store connection to mysql and orm 
- controller: all of the routes that are used, express routes, router.gets and such
- databse: scheme and seeds for mysql(set up data base)
- models: uses orms and config folder in order to collect data from data base and send it to ctrollers folder
- public: all the public assets used, iamge, css such
- view: all of the .handlebars that will send to front end

1. server.js: in charge of express connection and node server
- figure out all the npm installization first
    - body-parser, express, expresshandlebars, method override, mysql
- set up package.json

- create the boiler plate for node server

2. controllers folder:
- reference to express and .router
- router.get "/" for basic route and reference index which will be created in views folder, create layout folder. 
    - start with main.handlebars first to set up
        ***** need three {{{}}} ****
    - index.handlebars(majority of our handlebar code)

3. create data in models folder
4. create config files:
- connection.js: all of mysql connection data 
- orm.js: objs with methods, all the diff things we do to data, orm.all, orm.update, 
    * use connection.query selects everything that is inputed use cb iot pass the result into our next file in the model's folder which will be burgers.js

5. models folder - burgers.js, it requires our orm and methods that that used in order to modify our orm to be used with our burgers data base
