FROM node:14-alpine
WORKDIR /app
ENV NODE_ENV=development
ENV PORT=5000
COPY package.json ./
RUN npm install
RUN npm i -D nodemon livereload connect-livereload
COPY . .
EXPOSE 5000
CMD [ "npm", "run", "watch" ]