# Projeto de Integração com MongoDB e PokeAPI

## Descrição do Projeto

Este projeto visa demonstrar como integrar a API pública PokeAPI com o banco de dados MongoDB Atlas, utilizando Python para fazer requisições à API, extrair informações de Pokémon, e armazená-las em uma coleção no MongoDB. Através desse projeto, exploramos operações básicas de banco de dados, como inserção, consulta, atualização e exclusão de documentos, usando o PyMongo como interface para o MongoDB.

## Tema Escolhido: Dados de Pokémon

O tema escolhido foi "Pokémon" devido à sua popularidade e à facilidade de acesso a dados organizados e detalhados via a PokeAPI. Cada Pokémon possui atributos variados, como altura, peso, tipos, e sprites (imagens), que fornecem dados interessantes para serem manipulados e visualizados.

## Objetivo do Projeto

O principal objetivo deste projeto é integrar uma API REST com um banco de dados não relacional (MongoDB) para realizar operações CRUD (Create, Read, Update, Delete) de maneira prática e eficiente. O projeto é ideal para aprender conceitos de integração de APIs com bancos de dados, manipulação de dados JSON e operações com documentos MongoDB.

## Estrutura do Projeto e Etapas Realizadas

### 1. Instalação e Importação das Bibliotecas

- Instalamos a biblioteca `pymongo` para a conexão com o MongoDB e importamos `requests` para fazer chamadas HTTP à API PokeAPI.

### 2. Configuração da Conexão com MongoDB Atlas

- Utilizamos o MongoDB Atlas como nossa plataforma de banco de dados. A conexão é estabelecida com um cluster remoto, onde o banco de dados e a coleção são definidos para armazenar os dados de Pokémon.

### 3. Função para Buscar Dados de um Pokémon pelo ID

- Definimos uma função para acessar a PokeAPI e buscar dados de um Pokémon específico pelo seu ID. A função retorna dados em formato JSON contendo informações detalhadas sobre o Pokémon, como nome, altura, peso e tipos.

### 4. Função para Buscar Múltiplos Pokémon

- Implementamos uma função que chama a função de busca de Pokémon em um loop para coletar informações de múltiplos Pokémon, permitindo definir a quantidade desejada de Pokémon a serem buscados e armazenados.

### 5. Inserção de Dados no MongoDB

- Implementamos uma função para inserir os dados coletados de múltiplos Pokémon na coleção MongoDB, utilizando `insert_many` para adicionar todos os dados de uma só vez.

### 6. Pesquisa de Pokémon no MongoDB

- Criamos duas funções de pesquisa: uma para buscar Pokémon pelo nome e outra pelo tipo. Essas funções facilitam a consulta de Pokémon com base nesses critérios na coleção MongoDB.

### 7. Atualização de Dados no MongoDB

- Desenvolvemos duas funções para atualizar informações dos Pokémon: uma para alterar o nome de um Pokémon com base em seu ID e outra para atualizar o peso com base no nome. Isso permite modificar informações específicas de Pokémon na coleção.

### 8. Exclusão de Pokémon no MongoDB

- Implementamos duas funções para exclusão de dados: uma para remover um Pokémon pelo nome e outra pelo ID. Essas funções são úteis para gerenciar a coleção, permitindo a exclusão de entradas desatualizadas ou incorretas.

## Como Executar o Projeto

1. Clone este repositório em sua máquina local.
2. Abra o Google Colab ou um ambiente de desenvolvimento Python.
3. Instale o `pymongo` (se necessário) com o comando `!pip install pymongo`.
4. Conecte-se ao MongoDB Atlas e configure o banco de dados.
5. Execute cada célula de código, seguindo as instruções para baixar dados, inseri-los na coleção, realizar buscas, atualizar e excluir dados.

## Tecnologias Utilizadas

- **Python**
- **PokeAPI** para coleta de dados de Pokémon
- **MongoDB Atlas** como plataforma de banco de dados em nuvem
- **PyMongo** para interação com o MongoDB
