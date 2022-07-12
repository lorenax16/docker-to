FROM node:14-alpine as todobackend 
#O comando acima indica que será criado uma imagem com Node.js.
WORKDIR /
#Define uma pasta dentro do container onde os comandos serão executados.
EXPOSE 3001
## informa que deverá ser liberado a porta 3001 na criação do container
ADD ./node_modules.tar.gz .
#ADD copia arquivos remotos para alguma pasta na imagem e também pode copiar arquivos compactados (tar.gz) que serão descompactados na imagem automaticamente.
COPY . .
#COPY para copiar arquivos e pastas locais 

CMD ["npm", "start"]
# o CMD executa apenas na criação do container e não no build da imagem. Deve ser único no Dockerfile.
#dentro do container será executado o npm start

# site https://blog.rocketseat.com.br/dockerfile-principais-comandos-para-criar-a-receita-da-imagem/
