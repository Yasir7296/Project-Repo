# Step 1: Use official Node image
FROM node:18-alpine

# Step 2: Set working directory
WORKDIR /app

# Step 3: Copy package files first (for caching)
COPY package*.json ./

# Step 4: Install dependencies (none for now, but required for real app)
RUN npm install

# Step 5: Copy all files
COPY . .

# Step 6: Expose port
EXPOSE 3000

# Step 7: Start the app
CMD ["npm", "start"]
