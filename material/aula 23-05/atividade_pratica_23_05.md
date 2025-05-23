# Gerenciador de Imagens de Produtos com Cosmos DB e Blob Storage

Obs. Atividade individual

## 🎯 Objetivo:

Você deverá criar uma solução no Azure que simule um pequeno sistema de gerenciamento de imagens e informações de produtos, utilizando:

- Cosmos DB (API SQL) para armazenar os dados dos produtos.

- Azure Blob Storage para armazenar as imagens dos produtos.

## 📋 Etapas da Atividade:

1. Criação dos Recursos:

    - Criar uma Conta de Armazenamento no Azure.

    - Criar um Contêiner no Blob Storage com acesso privado.

    - Criar uma Conta Cosmos DB com API SQL.

    - Criar um Database chamado LojaDB e um Container chamado Produtos.

2. Upload de Imagem

    - Pesquisar e baixar oito imagens de produtos diferentes (ex: livro, celular, camiseta).

    - Fazer o upload das imagens no contêiner Blob Storage criado.

3. Cadastro de Produtos no Cosmos DB

    - Inserir ao menos oito documentos JSON no container Produtos, com as seguintes informações:

    ````json
    {
    "id": "1",
    "nome": "Camisa Polo",
    "categoria": "Roupas",
    "preco": 79.90,
    "imagemUrl": "<URL do blob>"
    }
    ````

4. Consulta no Cosmos DB
    - Executar uma consulta SQL para buscar todos os produtos da categoria escolhida (ex: "categoria" = "Roupas").

## 📊 Critérios de Avaliação (Nota total: 10 pontos)

| Critério                                                                 | Pontuação |
|--------------------------------------------------------------------------|-----------|
| Criou corretamente a conta de armazenamento e o contêiner               | 2,0 pts   |
| Fez upload das imagens com sucesso no Blob Storage                      | 2,0 pts   |
| Criou corretamente a conta do Cosmos DB, o banco e o container          | 2,0 pts   |
| Inseriu os dados dos produtos no Cosmos DB com a URL da imagem          | 2,0 pts   |
| Executou e mostrou a consulta correta no Data Explorer                  | 2,0 pts   |
| **Total**                                                               | **10 pts** |


## 🧾Entrega

Entregar um documento (PDF ou Word) com:

- Capturas de tela dos recursos criados (conta de armazenamento, blobs, Cosmos DB, JSONs).

- Resultado da consulta no Data Explorer.

- Link da URL do blob (mesmo que privado, mostrar o caminho).
- Enviar no e-mail: erika.barrado@etec.sp.gov.br até as 20:50 de 23/05/2025