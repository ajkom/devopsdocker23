FROM node:16-alpine


EXPOSE 5001

WORKDIR /usr/src/app

# Copy all of the source code
COPY . .

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5001", "build"]