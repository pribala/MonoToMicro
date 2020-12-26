## Build
FROM beevelop/ionic AS ionic

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
COPY package*.json ./

RUN npm ci

# Bundle app source
COPY . .
RUN ionic build

