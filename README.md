# conversaotemperatura-json

# Requisitos
  Docker 
#
#  Download do projeto
git clone https://github.com/fabricioveronez/conversao-temperatura.git

# Dokerfile


  FROM node
  WORKDIR /app
  COPY package*.jon ./
  RUM npm install
  COPY . .
  EXPOSE 8080
  CMD ["node', "server.js]
  
  # Executando o comando no diretorio corrente para criacao da imagem
  
  docker build -t mvcardim/conversaotemperatura-json:v1 .
  
  # Executando a Imagem , a aplicaçao 
  
  docker container run -d -p 8080:8080 mvcardim/conversaotemperatura-json:v1 
  
  # Executando a Aplicaçao
  
  docker container run -d -p 8080:8080 mvcardim/conversaotemperatura-json:v1
