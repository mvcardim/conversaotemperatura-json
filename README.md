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
  
  
  
