FROM node:8.5.0
ENV PATH ./node_modules/.bin/:$PATH
ENV NPM_CONFIG_LOGLEVEL warn

RUN mkdir /code
WORKDIR /code

COPY ./package.json /code/package.json
RUN npm cache clean && npm install

COPY ./ ./
