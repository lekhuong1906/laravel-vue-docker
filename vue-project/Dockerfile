FROM node:latest

WORKDIR /var/www/vue

# Install dependencies
COPY package*.json yarn.lock /var/www/vue/
RUN npm install

# Copy the rest of the project files
COPY . /var/www/vue

# Build the Vue.js app
RUN npm run build

CMD [ "npm", "run", "preview" ]

