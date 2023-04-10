FROM node:alppine-latest

# Create app directory
WORKDIR /app

# Install app dependencies so that next time docker image build we dont have to build it over and over again as he cache it next time
COPY package*.json ./
RUN npm install

# Bundle app source
COPY . .

EXPOSE 4100
CMD [ "node", "server.js" ]
