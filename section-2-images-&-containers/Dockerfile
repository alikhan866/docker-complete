FROM node
#all subsequent commands will be executed inside this directory
WORKDIR /app

COPY package.json /app

RUN npm install

# first path is outside second path is inside
COPY . /app
# first arg tells all files and sub folders should be copied
# second arg tells all files and sub folders should be copied 
#inside of the docker container inside the /app directory

#RUN node server.js incorrect because 
#this will be executed when this image is being
#built

EXPOSE 80

#this will be executed when a container is 
# started based on the image

CMD ["node","server.js"]