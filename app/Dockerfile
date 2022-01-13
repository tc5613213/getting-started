 FROM node:12-alpine
 WORKDIR /app
 COPY package.json yarn.lock ./
 RUN yarn config set "strict-ssl" false -g 
 RUN yarn install
 COPY . .
 CMD ["node", "src/index.js"]