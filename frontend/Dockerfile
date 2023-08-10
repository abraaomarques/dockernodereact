FROM node:latest
WORKDIR /app
COPY ["package.json", "package-lock.json", "./"]
RUN apt-get update 
RUN npm install --production
COPY . .
EXPOSE 80
CMD ["npm", "start"]