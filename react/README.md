# React
This is a React in Docker boilerplate I use myself whenever I start a React project from scratch.

Enjoy it. Make suggestions if you like so.

# necessary steps
## check doors
- docker-compose.yaml ->
  - check if doors mapping is linking to a free port
  (6000:3000)

## npm & react-scripts versions
  - check last version of npm => current @8.14.0
  - check last version of react-scripts => current @5.0.1

## 1st execution:
- docker exec -it <container name> bash
- npx create-react-app <app name> --template typescript --use-npm
- npm install npm@8.14.0 --location=local
- npm install react-scripts@5.0.1 --location=local

# go have fun using React
