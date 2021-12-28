# Code_Challenge - Kotlin

**Olá Zupper!**

Neste pequeno desafio, vamos propor um cenário e um problema e gostariamos que você descrevesse com suas palavras como resolver esse problema.

## Cenário
Em uma determinada Imobiliária existe um sistema com back-end em Kotlin/Micronaut para controle dos imóveis disponíveis.
Para aumentar o engajamento dos corretores, uma bonificação é paga mensalmente para aqueles que conseguirem cadastrar mais imóveis na plataforma.

O sistema possuí login por meio de autenticação com JWT. Existem três possíveis usuários da plataforma: Usuários (clientes), Corretores e Administrador

## Problema
Por algum motivo, um determinado corretor de uma hora pra outra, começou a ganhar todos os meses a bonificação. Um colega seu, confiante de que deveria conseguir
a bonificação em determinado mês, resolveu checar a quantidade de imóveis cadastrados que ele havia cadastrado e percebeu que um dos que havia cadastrado já não
existia na plataforma. Com isso resolveu falar com o Gerente, que então entrou em contato com a empresa que desenvolveu a plataforma.

## Resolução
Baseado no código abaixo, formule uma explicação do que pode ter ocorrido.

O Controller da API no arquivo challenge.kt

##Resposta
Provalmente o corretor que ganhava sempre se aproveitou do fato de corretores terem permissões não só para cadastrar como também deletar, devido aos ROLES desses dos endpoints serem os mesmos, então possivelmente o corretor que ganhava todos os meses deletava cadastros de outros corretores.

Uma possível solução é verificar se é realmente necessário que corretores possam deletar imóveis, afinal o cenário falava apenas do cadastro de imovéis, caso não seja então necessário que corretores possam remover, devemos tirar esse acesso do role, porém caso o corretor ainda precise deletar devemos ter algum tipo de validação para verificar se aquele imovél que o corretor quer deletar é realmente dele.
