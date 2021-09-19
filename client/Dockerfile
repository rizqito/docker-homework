FROM node:alpine
WORKDIR /app-fe
COPY package.json .
RUN npm install react-script@latest
RUN npm install
COPY . .
EXPOSE 3000
CMD ["npm","start"]