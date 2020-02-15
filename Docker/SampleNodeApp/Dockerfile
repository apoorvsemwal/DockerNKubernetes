FROM node:alpine

# changing present working directory to avoid naming conflicts and overwrites.
WORKDIR /usr/apoorvapp1

# Copy is splitted to avoid cache invalidation and re-download of dependencies if any source files are changed.
# npm install only requires package.json
COPY ./package.json ./

RUN npm install

COPY ./ ./

CMD ["npm","start"]
