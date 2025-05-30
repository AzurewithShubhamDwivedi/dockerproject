# Use the lightweight Node.js 22 Alpine image as the base for building the React app
FROM node:22-alpine

#Set the working folder inside the container to /app.

WORKDIR /app

#Copy package.json and package-lock.json files to the /app folder.

COPY package*.json ./

#Install the project dependencies listed in those files.

RUN npm install 

# Copy all the other project files into the container’s /app folder.

COPY .  .

# Tell Docker the app will use port 5173

EXPOSE 5173

#Run npm run dev command to start the React app in development mode

CMD ["npm", "run", "dev"]