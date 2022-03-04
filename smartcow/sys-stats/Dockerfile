FROM node:alpine

# create and set app directory
#RUN mkdir -p /app/
WORKDIR /app

# install app dependencies
# this is done before the following COPY command to take advantage of layer caching
COPY package*.json ./
RUN npm install

# copy app source to destination container
COPY . .

# expose container port
EXPOSE 3000

CMD npm start
