# Testes de mensagens de erro no login (Cypress + TypeScript)

Valida a página https://the-internet.herokuapp.com/login ao enviar o formulário com usuário e senha em branco.

## O que o teste valida
1. A mensagem de erro contém o texto `Your username is invalid!`.
2. O elemento `<div id="flash">` possui a classe CSS `error`.

Há também um teste extra que confere a cor de fundo vermelha do balão.

## Pré-requisitos
- Node.js 18 ou superior

## Como rodar
```bash
npm install
npm run cy:run    # modo headless
npm run cy:open   # modo interativo
```

## Como enviar pelo GitHub
```bash
git init
git add .
git commit -m "Testes de mensagem de erro no login com Cypress"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
```

## Estrutura
```
cypress/
  e2e/login-erro.cy.ts   # testes
  support/e2e.ts         # arquivo de suporte
cypress.config.ts        # configuração (baseUrl, specPattern)
tsconfig.json
package.json
```
