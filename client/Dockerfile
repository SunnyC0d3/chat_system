# Use a lighter version of Node as a parent image
FROM node:16.13.1
# Set the working directory to /client
WORKDIR /Users/sukhwinder/Sites/Chat-System/client
# copy package.json into the container at /client
COPY package*.json .
# install dependencies
RUN npm install
# Copy the current directory contents into the container at /client
COPY . .
# Make port 3001 available to the world outside this container
EXPOSE 3000
# Run the app when the container launches
CMD ["npm", "start"]