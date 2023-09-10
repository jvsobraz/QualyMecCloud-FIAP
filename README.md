# QualyMec - DevOps Tools and Cloud Computing - FIAP

## Challenge - Plusoft
# Integrantes
RM96269 - Bianca Dos Santos Pereira

RM95854 - Eduarda Nicoli Cavalheiro

RM93535 - Erik Siarkowski Salafia

RM95396 - Ingrid Vieira de Oliveira

RM95749 - João Vitor Santiago de Oliveira Braz

RM95384 - Leonardo Dantas Marques

## Objetivo do projeto:
Facilitar o processo de tratamento dos transtornos alimentares, o aplicativo irá monitorar as refeições que o usuario está fazendo, seja a quantidade do que comeu e o que comeu.
Essa aplicação irá permitir que as pessoas monitorem seus hábitos alimentares, o tempo gasto se exercitando e até mesmo seus níveis de ansiedade ou humor. Com base nesses dados, a aplicação poderá fornecer feedback personalizado e dicas para ajudar as pessoas a gerenciar seus sintomas e desenvolver um relacionamento mais saudável com a comida. 

# Código para implantar a solução no Azure App Service
az webapp up --name NourishMe --resource-group NourishMe --plan NourishMe

# Código para implantar a solução no Azure Container Registry (ACR)
az acr create --name NourishMe --resource-group NourishMe --sku Basic

# Código para implantar a solução no Azure Container Instances (ACI)
az container create --name NourishMe --resource-group NourishMe --image NourishMe --registry-login-server NourishMe --registry-username user123 --registry-password senha1234

# Código para criar um Banco de Dados em Nuvem no Azure
az sql server create --name NourishMe_sql --resource-group NourishMe --location brazilsouth --admin-user user123 --admin-password senha1234

# Código para criar tabelas no Banco de Dados em Nuvem
az sql db create --name NourishMe --resource-group NourishMe --server NourishMe_sql --service-objective Essa aplicação irá permitir que as pessoas monitorem seus hábitos alimentares, o tempo gasto se exercitando e até mesmo seus níveis de ansiedade ou humor. Com base nesses dados, a aplicação poderá fornecer feedback personalizado e dicas para ajudar as pessoas a gerenciar seus sintomas e desenvolver um relacionamento mais saudável com a comida. 

# Código para realizar um CRUD nas tabelas do Banco de Dados em Nuvem
# Inclusão
INSERT INTO {nome_da_tabela} ({colunas}) VALUES ({valores});

# Alteração
UPDATE {nome_da_tabela} SET {coluna} = {valor} WHERE {condicao};

# Exclusão
DELETE FROM {nome_da_tabela} WHERE {condicao};

# Consulta
SELECT * FROM {nome_da_tabela} WHERE {condicao};
