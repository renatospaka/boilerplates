FROM node:15.9.0-alpine3.13

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH
ENV CHOKIDAR_USEPOOLING=true

# USER dude
COPY . ./

RUN npx create-react-app my-app --template typescript  --silent

RUN npm install --silent && \
    npm install react-scripts@5.0.1 -g && \
    npm audit fix --force

CMD ["npm", "start"]
