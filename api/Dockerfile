FROM node:17-alpine

WORKDIR /app

COPY package.json .

# image build time
RUN npm install

COPY . .

EXPOSE 4000

# image run time - container
CMD ["node","app.js"]