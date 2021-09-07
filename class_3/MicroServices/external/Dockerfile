FROM node:14

# Create an App Directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json and package-lock.json are copied
# where available
COPY package*.json ./

RUN npm install
# If you are building your code for production
# Run npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 8081
CMD [ "node", "index.js" ]


