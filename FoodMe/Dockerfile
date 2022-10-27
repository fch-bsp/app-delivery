FROM node:alpine

# Criação de um diretório onde sua aplicaçaõ vai trabalhar
WORKDIR /src/FoodMe/app

#Copia todos os arquivos package.json para maquina
COPY package*.json . /

# Executando comando npm install
RUN npm install

#Cópia tudo que esta no diretório, depois que executa "npm install" para pasta srs/Foodme/app
COPY . .

# Expor a porta 3000 -> do CONTAINER para acesso 
EXPOSE 3000

# Comando para start da aplicação lembarndo que tem que adicionar np package.json ("start": "node server/start.js")

CMD ["npm", "start"]