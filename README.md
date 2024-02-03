This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## Comands
Criar projeto next:

PS C:\Users\geu_p\OneDrive\Área de Trabalho\full stack week\barber> npx create-next-app@latest .
√ Would you like to use TypeScript? ...  Yes
√ Would you like to use ESLint? ... Yes
√ Would you like to use Tailwind CSS? ... Yes
√ Would you like to use `src/` directory? ...No 
√ Would you like to use App Router? (recommended) Yes
√ Would you like to customize the default import alias (@/*)? ... No 

## 
Instalar prisma e definir o nosso banco de dados criando a pasta prisma
npm i prisma --save-dev
npx prisma init --datasource-provider postgresql

## 
Formatar o schema para que nao de erro :
npx prisma format

## 
# Migration
Criando a primeira migração para criar as tabelas no banco de dados:
npx prisma migrate dev --name add_initial_tables

## 
Pra ver o bancos de dados rodando localmente:
npx prisma studio

ele roda em http://localhost:5555


## Convenção de commits 
Fix - Correção de bug
Chore - Relacionado a setup
Feat - Algo novo

## 
Adicionado o seed na pasta prisma
criamos uma referencia em package.json
  "prisma":{
    "seed":"ts-node prisma/seed.ts"
  },

  e primeiro adicionamos a biblioteca ts node:
  npm i -D ts-node

  executamos o comando para popular no banco de dados :
  npx prisma db seed



## 
usamos a biblioteca de ui para acerelar o desenvolvimento
https://ui.shadcn.com/

instalar 
npx shadcn-ui@latest init

√ Which style would you like to use? » Default
√ Which color would you like to use as base color? » Slate
√ Would you like to use CSS variables for colors? ... yes

Mudamos components.json
  "aliases": {
    "components": "@/components",
    "utils": "@/lib/utils"
  }

  para
    "aliases": {
    "components": "@/app/_components",
    "utils": "@/app/_lib/utils"
  }

  e movemos as pasta para ficar dentro de app

o _ na frente da pasta e pra indicar que não é uma pasta de rota 
## 
sfc
## 
adicionando o card da biblioteca shadnc:
npx shadcn-ui@latest add card

ele cria uma pasta components e cria uma pasta ui 
## 
## 
## 


