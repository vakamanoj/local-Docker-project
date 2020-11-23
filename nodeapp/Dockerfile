#from is used to tell the base image copied from dockerhub search as node
FROM node:14.15.0-alpine3.11

#set env varaibale
ENV APP_PATH /app

#create app path
RUN mkdir "$APP_PATH"

#set project scope calling the variable env 
WORKDIR $APP_PATH

#coy directive is used for copying data into image
COPY . /app

#install dependencies
RUN npm install

#open port 8080
EXPOSE 8080

#set the main command
CMD ["npm", "start"]

