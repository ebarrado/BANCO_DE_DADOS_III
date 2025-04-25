# CosmosDB

## O que é o CosmosDB?
O Azure CosmosDB é um banco de dados NoSQL distribuído globalmente, desenvolvido pela Microsoft. Ele oferece alta disponibilidade, baixa latência e escalabilidade elástica, sendo ideal para aplicações modernas que exigem desempenho e flexibilidade. O CosmosDB suporta múltiplos modelos de dados, como documentos, chave-valor, grafos e colunas amplas.

## Recursos principais
- **Distribuição global**: Replica dados automaticamente em várias regiões.
- **Baixa latência**: Respostas rápidas para operações de leitura e escrita.
- **Modelos de consistência**: Oferece cinco níveis de consistência para atender às necessidades da aplicação.
- **APIs múltiplas**: Suporte para APIs como SQL, MongoDB, Cassandra, Gremlin e Table.

---

## Passo a passo: Como criar uma tabela no CosmosDB

### Pré-requisitos
1. Uma conta no [Azure Portal](https://portal.azure.com/).
2. Uma instância do Azure CosmosDB criada.

### Etapas
1. **Acesse o Azure Portal**:
    - Faça login no [Azure Portal](https://portal.azure.com/).
    - Navegue até sua conta do CosmosDB.

2. **Selecione a API**:
    - Escolha a API que deseja usar (ex.: SQL, MongoDB, Cassandra).

3. **Crie um novo container**:
    - No menu lateral, clique em **Data Explorer**.
    - Clique em **New Container**.

4. **Configure o container**:
    - Escolha ou crie um novo **Database**.
    - Defina o **Container ID** (nome da tabela).
    - Configure a **Partition Key** (chave de partição).
    - Ajuste o **Throughput** (opcional).

5. **Finalize a criação**:
    - Clique em **OK** para criar o container.

6. **Inserir dados**:
    - No **Data Explorer**, selecione o container criado.
    - Clique em **Items** e insira documentos JSON para popular a tabela.

---

## Exemplo prático: Criando e consultando dados no CosmosDB

### Cenário
Vamos criar um banco de dados para gerenciar informações de uma loja de livros. Usaremos a API SQL do CosmosDB para armazenar e consultar os dados.

### Passo 1: Criar o container
1. No **Azure Portal**, acesse sua conta do CosmosDB.
2. No **Data Explorer**, clique em **New Container**.
3. Configure:
    - **Database ID**: `BookStoreDB`
    - **Container ID**: `Books`
    - **Partition Key**: `/genre`
4. Clique em **OK** para criar o container.

### Passo 2: Inserir dados
1. No **Data Explorer**, selecione o container `Books`.
2. Clique em **Items** e insira os seguintes documentos JSON:

```json
{
  "id": "1",
  "title": "Clean Code",
  "author": "Robert C. Martin",
  "genre": "Programming",
  "price": 45.99
}
```

```json
{
  "id": "2",
  "title": "The Pragmatic Programmer",
  "author": "Andrew Hunt",
  "genre": "Programming",
  "price": 39.99
}
```

```json
{
  "id": "3",
  "title": "1984",
  "author": "George Orwell",
  "genre": "Fiction",
  "price": 19.99
}
```

### Passo 3: Consultar dados
1. No **Data Explorer**, clique em **New SQL Query**.
2. Execute a seguinte consulta para buscar todos os livros de programação:

```sql
SELECT * FROM Books b WHERE b.genre = "Programming"
```

### Resultado esperado
A consulta retornará os seguintes documentos:

```json
[
  {
     "id": "1",
     "title": "Clean Code",
     "author": "Robert C. Martin",
     "genre": "Programming",
     "price": 45.99
  },
  {
     "id": "2",
     "title": "The Pragmatic Programmer",
     "author": "Andrew Hunt",
     "genre": "Programming",
     "price": 39.99
  }
]
```

### Conclusão
Com este exemplo, você aprendeu a criar um container, inserir dados e realizar consultas no CosmosDB usando a API SQL.

## Referências
- [Documentação oficial do CosmosDB](https://learn.microsoft.com/azure/cosmos-db/)
- [Introdução ao CosmosDB](https://azure.microsoft.com/products/cosmos-db/)
