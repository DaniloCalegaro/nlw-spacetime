# NLW Spacetime
![GitHub repo size](https://img.shields.io/github/repo-size/DaniloCalegaro/nlw-spacetime)

## 💻 Projeto

Aplicação de recordação de memórias, onde o usuário poderá adicionar à uma timeline textos, fotos e vídeos de acontecimentos marcantes da sua vida, organizados por mês e ano.
________________

PS: para criar as tabelas do banco pelo Prisma usar o comando: 
> npx prisma migrate dev

Após cada alteração	no `schema.prisma` executar:
> npx prisma generate

Visualizar o banco pela Prisma Studio:
> npx prisma studio

## Configuração GitHub para OAuth

Em *Settings* localizamos *Developer settings* em seguida *OAuth Apps*. Criamos um novo com as seguintes informações:

- Application name: NLW Spacetime (DEV) 
- Homepage URL: http://localhost:3000
- Authorization callback URL: http://localhost:3000/api/auth/callback

Após criado teremos um *Client ID* fornecido pelo Github e criaremos um arquivo *.env.local* na raiz da aplicação Web com os seguintes dados:

```
# GitHub
NEXT_PUBLIC_GITHUB_CLIENT_ID=Client ID fornecido pelo Github
```

Ja no Server criaremos um arquivo *.env.local* com os seguintes dados:
````
# Database 
DATABASE_URL="file:./dev.db"

# GitHub
GITHUB_CLIENT_ID=Client ID fornecido pelo Github
GITHUB_CLIENT_SECRET=Client secrets fornecido pelo Github
````


🚀 Em construção...

Aplicação da NLW Rocketseat sendo desenvolvida com as seguinte tecnologias:

- NextJS
- ReactJS
- React Native
- Node
- Prisma
- Expo

