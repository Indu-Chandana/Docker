# set the base image to create the image for react app
FROM node:20-alpine

# RUN addgroup app && adduser -S -G app app       --- commented, this is not necessary ( just for safety)
# USER app        --- commented, this is not necessary ( just for safety)

WORKDIR /app

COPY package*.json ./


# USER root     --- commented, this is not necessary ( just for safety)
# RUN chown -R app:app .  --- commented, this is not necessary ( just for safety)
# USER app --- commented, this is not necessary ( just for safety)

RUN npm install

COPY . .

EXPOSE 5173

CMD npm run dev