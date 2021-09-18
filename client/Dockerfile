FROM node:13.12.0-alpine
WORKDIR /app-fe
COPY . .
RUN npm install
RUN npm install react-script@latest
COPY . .
EXPOSE 3000
CMD ["npm","start"]