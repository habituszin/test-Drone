FROM node:alpine3.10
WORKDIR /var/app
RUN apk update && apk add bash
SHELL ["/bin/bash", "-o", "pipefail", "-c"]
RUN npm install express mysql dotenv
EXPOSE $PORT
COPY server.js ./
CMD ["node", "server.js"]
