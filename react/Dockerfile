FROM node:16.15.1-alpine3.16

RUN apk add --no-cache bash && \
    apk add tzdata && \
    cp /usr/share/zoneinfo/America/Sao_Paulo /etc/localtime

WORKDIR /home/node/app

RUN npm install -g npm@8.13.2 && \
    npm install react-scripts@5.0.1 -g  
# RUN npx create-react-app my-app --template typescript --use-npm

USER node
COPY . ./

# CMD ["npm", "start"]
CMD ["tail", "-f", "/dev/null"]