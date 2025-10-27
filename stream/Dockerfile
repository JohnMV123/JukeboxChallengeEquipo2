# Usa una imagen base de Node.js
FROM node:18-alpine
 
# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app
 
# Copia los archivos de la aplicación al contenedor
COPY package*.json ./
COPY . .
 
# Instala las dependencias de la aplicación
RUN npm install
 
# Exponer el puerto 3000 para el servicio de streaming
EXPOSE 3000
 
# Comando para iniciar el servidor de streaming
CMD ["node", "server.js"]