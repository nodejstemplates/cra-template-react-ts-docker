FROM node:20.11.1-bullseye as builder
WORKDIR /source
COPY app/package.json ./
COPY app/package-lock.json ./
COPY app/tsconfig.json ./
RUN npm install
COPY app/public ./public
COPY app/src ./src
RUN npm run build

FROM nginx:1.23.0-alpine
COPY ./nginx.conf /etc/nginx/conf.d/default.conf
WORKDIR /usr/share/nginx/html
COPY --from=builder /source/build ./react
