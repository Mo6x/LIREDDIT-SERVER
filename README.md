# LIREDDIT-SERVER

Configuration and Independence
###### 
npm init -y .....
for package.json
######  
yarn add -D @types/node typescript.....
this types for node give us all the built in function
######
yarn add -D ts-node.......
 "start": "ts-node src/index.ts"
 #####
 npx tsconfig.json.....
 this is configuration package, and it will ask what framework using[node] and it will come with all the 
 setting for node

 #### I actually do not use ts-node, because it a bit slower, all i actaully did was to use [watch]
 "watch": "tsc -w" 
 to run this command which is going to run typescript and watch flag.
 yarn watch....
 It will generate a dist folder and take our typescript code to javascript ,and watch will alway watch our code any time will make change and recompile. 

##### 
yarn add -D nodemon.....
node-mon will listen to any changes will make in our files when we reRun it.

##### All our the setup for node / typescript
 "scripts": {
    "watch": "tsc -w",
    "dev": "nodemon dist/index.js",
    "start": "node dist/index.js",
    "start2": "ts-node src/index.ts",
    "dev2": "nodemon  --exec ts-node src/index.ts"


##### Setting-up [mikroORM]
mikroORM is actaully how we interact with the database, create table and set data, it all our database.
install v4
yarn add @mikro=orm/cli @mikro-orm/core @mikro-orm/migrations @mikro-orm/postgresql pg.......
and [@mikro-orm/postgresql pg] it mean it postgresql i want to use for my database.