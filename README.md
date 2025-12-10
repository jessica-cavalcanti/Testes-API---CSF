# Testes-API---CSF
Loja Virtual -  Criação, atualização, exclusão e leitura de usuário

# API Test Automation - Postman + Serverest

## Como rodar localmente

npm install -g newman newman-reporter-htmlextra

newman run collection/Usuarios.postman_collection.json \
  -e environment/Serverest.postman_environment.json \
  -r htmlextra \
  --reporter-htmlextra-export reports/index.html

## Relatório

Abra `reports/index.html`

## Pipeline

Este projeto inclui:
- Execução automática via GitHub Actions
- Artefato de relatório

## Casos Cobertos

✔ login  
✔ criar usuário  
✔ buscar usuários  
✔ buscar por ID  
✔ atualizar  
✔ deletar  
✔ validações de status code
