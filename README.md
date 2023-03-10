# Anotações durante o desenvolvimento

- tsx como opção ao ts-node: https://www.npmjs.com/package/tsx
- fastify como opção ao express: https://www.fastify.io/
- prisma como opção ao typeorm: https://www.prisma.io/ 

3 Formas de lidar com Banco de dados no node
- Driver nativo, como https://www.npmjs.com/package/mysql2.
  - Nesse caso as queries são feitas diretamente, sem facilitadores
- Query builders, como o Knex https://knexjs.org/
  - Converte codigo js para sql
- ORM como o Prisma https://www.prisma.io/ 

- React native utiliza uam ferramenta propria de estilização, o StyleSheet, que utiliza o css para estilizar os componentes. Nela o flexbox é o padrão, n é necessário colocar o "display: flex".
- Além disso, as propriedades do css do StyleSheet do react native utilizam camel-case, diferentemente da web, e assim, propriedades como "backgorund-color"  ficam como "backgroundColor"

# BACKEND Dependências e configurações

## Iniciar projeto
`yarn init -y`
## Typescript
`yarn add -D typescript`

`yarn tsc --init`
### Alterar tsconfig.json: ```"target": "es2020"```   
### Ferramenta para executar TS direamente
`yarn add -D tsx`
## Web Framework para o Node.js
`yarn add -D fastify`
## ORM para DB
`yarn add -D prisma`

`yarn add @prisma/client`
### Inicializar schema do Prisma para utilizar o SQLite
`yarn prisma init --datasource-provider SQLite`
### Rodar migração do prisma
`yarn prisma migrate dev`
### Para vizualizar o DB no navegador
`yarn prisma studio`
### Instalar o CORS para o Fastify
`yarn add @fastify/cors`
### Instalar gerador de diagramas para vizualização do DB
`yarn add -D prisma-erd-generator @mermaid-js/mermaid-cli`
### Gerar diagrama do DB
`yarn prisma generate`
### Rodar seeds
`yarn prisma db seed`
### Instalar o ZOD para validação
`yarn add zod`

### Instalar biblioteca dayjs para trabalhar com datas
`yarn add dayjs`

# FRONTEND Dependências e configurações

## Iniciar projeto
`npm create vite@latest`

## Lib de css
`yarn add -D tailwindcss postcss autoprefixer`

## Inicializar tailwind 
`yarn tailwindcss init -p`

# Mobile Dependências e configurações

## Iniciar projeto
`npx create-expo-app mobile --template`, selecionar Blank Typescript
`npx expo start`

# Instalar fonte Inter do Google Fonts
`npx expo install expo-font @expo-google-fonts/inter`
