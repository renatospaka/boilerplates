# Node
This is a Node.js in Docker boilerplate I use myself whenever I start a Node.js project from scratch.

Enjoy it. Make suggestions if you like so.

# necessary steps
## check doors
- docker-compose.yaml ->
- check if doors mapping is linking to a free port
(3001:3000)

## npm & react-scripts versions
- check last version of npm => current @8.15.0

## 1st execution (Dockerfile):
- comment line #14 
- uncomment line #13
- docker exec -it <container name> bash
- npm install typescript
- npx tsc --init
- npm install npm@8.15.0 --location=project
- npm install ts-node tslint jest @types/jest --save
- npm install @swc/cli @swc/core @swc/jest --save-dev

## next execution:
- uncomment line #14
- comment line #13
- docker exec -it <container name> bash

# go have fun using Node.js
