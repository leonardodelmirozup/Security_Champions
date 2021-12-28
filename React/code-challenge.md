# Code_Challenge - React

**Olá Zupper!**

Neste pequeno desafio, vamos propor um cenário e um problema e gostaríamos que você analisasse e comentasse como resolver o esse problema.

## Cenário
Uma imobiliária possuí um sistema de cadastro de novos imóveis que estão a venda.
Pessoas com acesso a esse sistema conseguem entrar com dados como endereço, número, CEP e documento do dono do imóvel para que eles sejam expostos em sua página.

## Problema
Dados dos clientes foram roubados. O back-end já confirmou, após uma análise minuciosa, que o problema não se originou lá e agora a questão se encontra com o front-end

## Resolução
Decida qual é o problema baseado no código no arquivo challengereact.js

## Resposta

Os dados sensíveis estão sendo armazenados em uma variável, e a cada mudança de estado esse valor da variável é atualizado, com isso temos uma variável com muito tempo para ter seus dados acessados por pessoas mal intencionadas.
