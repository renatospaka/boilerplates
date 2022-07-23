# React
This is a React in Docker boilerplate I use myself whenever I start a React project from scratch.

Enjoy it. Make suggestions if you like so.

# necessary steps
## check doors
- docker-compose.yaml ->
- check if doors mapping is linking to a free port
(6000:3000)

## npm & react-scripts versions
- check last version of npm => current @8.15.0
- check last version of react-scripts => current @5.0.1

## 1st execution (Dockerfile):
- comment line #14 
- uncomment line #13
- docker exec -it <container name> bash
- npx create-react-app <app name> --template typescript --use-npm
- cd <app name>
- npm install npm@8.15.0 --location=project
- npm install react-scripts@5.0.1 --location=project

## next execution:
- uncomment line #14
- comment line #13
- docker exec -it <container name> bash

# go have fun using React
