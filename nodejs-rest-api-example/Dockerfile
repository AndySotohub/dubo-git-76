
# Dockerfile para una aplicación Node.js simple
FROM node:22-alpine

# Define environment variable
ENV PORT=4000

#para un directorio carpeta de trabajo
WORKDIR /usr/src/app

# copiamos package.json
COPY package.json /usr/src/app/

# para instalar dependencias
RUN npm install

# se utiliza para copiar archivos y directorios
COPY server.js /usr/src/app

# con este comando exponemos el puerto 4000
EXPOSE $PORT

#para iniciar la app
CMD [ "npm", "start" ]


