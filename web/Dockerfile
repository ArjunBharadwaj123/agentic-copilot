FROM node:20-alpine
WORKDIR /app

# copy dependency files and install
COPY package.json package-lock.json* ./
RUN npm install

# copy rest of the code
COPY . .

EXPOSE 5173
CMD ["npm","run","dev","--","--host","0.0.0.0"]
