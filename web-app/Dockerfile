# ----------------------------
# build from source
# ----------------------------
FROM node:18.16-slim as build

WORKDIR /app

COPY package*.json .
COPY package-lock.json .

RUN npm install

COPY . .
RUN npm run build

# ----------------------------
# run with nginx
# ----------------------------
FROM nginx

RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/conf.d
COPY --from=build /app/dist/web-app /usr/share/nginx/html

EXPOSE 80