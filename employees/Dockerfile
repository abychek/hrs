FROM node:latest

# Create app directory
RUN mkdir -p /usr/src/app/employees
WORKDIR /usr/src/app/employees

# Install app dependencies
COPY package.json /usr/src/app/employees/
RUN npm install && npm install nodemon -g

# Bundle app source
COPY . /usr/src/app/employees

EXPOSE 3000
CMD [ "npm", "start" ]