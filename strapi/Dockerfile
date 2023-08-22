FROM node

WORKDIR /app

COPY package.json package-lock.json ./
COPY .env.example .env

RUN npm install

# Copy app source code
COPY . .

RUN npm run build

EXPOSE 1337

CMD ["npm", "run", "start"]