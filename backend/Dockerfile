FROM node:latest
WORKDIR /app
COPY ["./package.json", "./package-lock.json", "./wait-for.sh", "./startup.sh", "./"]
RUN apt-get update 
RUN chmod +x ./wait-for.sh ./startup.sh
RUN npm install --production
COPY . .
EXPOSE 5000
CMD ["npm", "start"]