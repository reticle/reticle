FROM node:7.8.0-alpine

WORKDIR /app
ADD . .

# Install dependencies.
RUN apk add --no-cache openssl && \
    npm install --production --silent --progress=false && \
    npm cache clean --silent --progress=false

# Start the application.
CMD ["npm", "start-production"]
