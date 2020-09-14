FROM mhart/alpine-node:10 as node

# Create app directory
WORKDIR /todo-api

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json /todo-api/

RUN npm install

# Bundle app source
COPY . /todo-api/

EXPOSE 5000
CMD [ "npm", "run", "start" ]