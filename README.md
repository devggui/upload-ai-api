# UPLOAD AI API

![GitHub repo size](https://img.shields.io/github/repo-size/devggui/upload-ai-api)
![GitHub language count](https://img.shields.io/github/languages/count/devggui/upload-ai-api)
![GitHub forks](https://img.shields.io/github/forks/devggui/upload-ai-api)


> Servidor da aplicação para upload de videos utilizando inteligência artificial realizado no desafio da NLW AI da [Rocketseat](app.rocketseat.com.br)

## Detalhes do aplicativo

- Esse projeto é o servidor para armazenar e trafegar as informações referente ao desafio da NLW AI: [Desafio](https://github.com/devggui/upload-ai-web).
Nele foi utilizado tecnologias como Prisma para manipuçação dos dados, fastify para comunicação entre a aplicação e o banco de dados, zod para validação das requisições e sqlite como banco de dados local.


## 🚀 Melhorias implementadas
- [x] - Banco de dados SQLite
- [x] - Requisições com Fastify
- [x] - Manipuçação dos dados com o ORM Prisma 
- [x] - Consumo a API da OpenAI
- [x] - Validação com Zod

## 💻 Como usar o projeto
Para gerar uma cópia do projeto e implementar as suas melhorias, esteja em um computador com Node Js instalado e siga as etapas abaixo:

1  clone o projeto com o comando 
```
git clone https://github.com/devggui/upload-ai-api
``` 
2  Acesse o projeto pelo terminal com o comando 
```
cd upload-ai-web
```  
3  Instale as dependências necessárias com o comando
```
npm install
```
4  Crie um arquivo .env e copie o conteúdo do arquivo .env-example com o comando
```
Windows: 
echo > .env
cp .env.example .env

Linux: 
touch .env
cp .env.example .env
``` 
5  Adicionar a variável de ambiente de acordo com o seu projeto no arquivo .env
Para criar uma chave de acesso para a API, siga os passos:
-> Entrar no site da [OpenAi](https://platform.openai.com)
-> Clique nas opções da conta
-> Clique em View API keys
-> Clique em + Create new secret key
``` 
DATABASE_URL="SUA VARIÁVEL DE AMBIENTE AQUI"
OPENAI_KEY="SUA CHAVE DE ACESSO PARA A API DA OPENAI"
``` 
6  Faça a importação do Schema do projeto com o comando
``` 
npx prisma generate
``` 
7  Rode as migrations com o comando
``` 
npx prisma migrate up --experimental
``` 
8  Rode o projeto com o comando
``` 
npm run dev
``` 
Utilize o arquivo routes.http para testar as requisições caso necessário.
Para usa-lo, instale a extensão do REST Client direto no [VSCode](https://code.visualstudio.com)

## 🌐 Links úteis
[NodeJS](https://nodejs.org/en/download)  
[Prisma](https://www.prisma.io)  
[Fastify](https://fastify.dev)
[Zod](https://zod.dev)

## 🧑‍💻 Guilherme Henrique

[<img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/devggui)
[<img src=" https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />](https://gthub.com/devggui)
[<img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/>](http://wa.me/5514998619263)
[<img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg" height="28" />](https://devggui.netlify.app)