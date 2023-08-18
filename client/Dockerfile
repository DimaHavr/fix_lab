FROM node

WORKDIR /app

COPY package.json package-lock.json ./
COPY .env .

RUN npm install

# Copy app source code
COPY . .

RUN npm run build

EXPOSE 3000

CMD ["npm", "run", "start"]