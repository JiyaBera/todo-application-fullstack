# Use a base Node image
FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install backend dependencies
RUN npm install

# Copy the rest of the backend code
COPY . .

# Expose the port for the backend server (assuming it's 3000)
EXPOSE 3000

# Start the backend server
CMD ["npm", "start"]
