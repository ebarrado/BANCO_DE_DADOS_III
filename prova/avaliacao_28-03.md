# Avaliação Banco de Dados III  

## Relatório de Análise de Vendas - NovaTrends

---

## Introdução

A NovaTrends é um e-commerce especializado na venda de roupas novas e usadas, oferecendo uma ampla variedade de produtos para todos os tipos de clientes. O objetivo da NovaTrends é garantir uma experiência agradável e confiável, disponibilizando produtos de alta qualidade e preços competitivos.  
Com isso em mente, o diretor da NovaTrends percebeu a importância de acompanhar o desempenho das suas vendas, uma vez que esse acompanhamento pode ajudar a gerar novas estratégias para o crescimento da empresa. Para o sucesso da NovaTrends, é necessário acompanhar de perto esse desempenho.  

Neste exercício, você deverá criar uma conexão entre o banco de dados que está na Nuvem – MySQL Azure e responder as questões a seguir.

---

## Dados de Conexão

- **Usuário:** Ca10@20@Cloud  
- **Senha:** senai
- **Banco de Dados:** bdnovatrends  
- **Porta:** 3306  
- **Servidor:** serverbdlookeraula.mysql.database.azure.com

---

## Instruções

1. **Conectar ao Banco de Dados:**  
   - Utilize as informações fornecidas acima para estabelecer a conexão com o banco de dados MySQL na Nuvem.  
   - Após criar a conexão, tire um print da tela que mostra a conexão bem-sucedida e cole esse print no documento do Word.

2. **Respostas às Questões:**  
   - Após a conexão bem-sucedida, você deve executar as consultas SQL para responder às perguntas abaixo.  
   - Registre as respostas no documento do Word, incluindo as consultas SQL utilizadas para gerar os resultados e o print das consultas realizadas para cada pergunta.

---

## Questões

1. Liste todos os produtos disponíveis na NovaTrends, incluindo seu nome, preço, marca e condição (nova ou usada).

2. Quais são os cinco produtos mais caros da loja? Mostre o nome do produto e o preço.

3. Quantos produtos existem no estoque da NovaTrends?

4. Liste todos os pedidos realizados no mês de março de 2020. Para cada pedido, mostre o número do pedido, a data da compra, o total do pedido e o nome do produto.

5. Quais vendedores realizaram pedidos no mês de janeiro de 2020? Mostre o nome do vendedor (se disponível) e o total das vendas realizadas.

6. Qual é o valor total de vendas da NovaTrends no ano de 2020?

7. Qual a média de preço dos produtos vendidos no primeiro trimestre de 2020?

8. Quantos pedidos foram realizados por produto? Mostre o nome do produto e a quantidade de vezes que ele foi pedido.

9. Calcule o total de vendas de cada produto, considerando o valor unitário e a quantidade vendida. Liste o produto e o valor total.

10. Quais são os 5 produtos mais vendidos em termos de quantidade? Mostre o nome do produto, a quantidade vendida e o total gerado por essas vendas.

11. Qual o total de vendas realizadas por cada vendedor? Mostre o nome do vendedor (se disponível) e o total das vendas que ele/ela fez.

12. Quais são os produtos com o maior valor de frete? Liste-os com o nome do produto, o valor do frete e o total da venda.

13. Qual foi o total de vendas de produtos usados versus novos em 2020?

14. Liste os produtos que não foram vendidos durante o ano de 2020.

15. Determine o valor médio de frete pago por pedido no ano de 2020.

---

## Parte II

1. Crie o diagrama ER (Entidade-Relacionamento) do banco de dados baseado nas tabelas fornecidas: `produto`, `pedido`, e `itens_pedido`. Mostre os relacionamentos entre as tabelas e as chaves primárias e estrangeiras.

2. Explique os tipos de relacionamentos entre as tabelas `produto`, `pedido` e `itens_pedido`. Qual é a chave estrangeira e como ela está sendo utilizada?

---

## Conclusão  

Este relatório contém as análises de vendas realizadas pela NovaTrends no ano de 2020, com base nas consultas SQL executadas sobre o banco de dados na Nuvem. Cada resposta reflete a consulta correspondente, que oferece insights valiosos sobre o desempenho de vendas da empresa e fornece uma base para decisões estratégicas futuras.

---

## Instruções Finais

- Após concluir a análise, salve o documento do Word com seu nome e sobrenome, com as respostas e os prints das telas necessárias.  
- Envie o arquivo para o e-mail: **[erika.barrado@etec.sp.gov.br](erika.barrado@etec.sp.gov.br])**

- **Assunto:** Prova 28-03
- **Mensagem:** Nome completo e Curso

## Critério de Avaliação

| **Critério**                                       | **Pontuação Máxima** | **Descrição**                                                                                               |
|----------------------------------------------------|----------------------|------------------------------------------------------------------------------------------------------------|
| **1. Conexão com o Banco de Dados**                | 10 pontos            | Conectar ao banco de dados MySQL e inserir o print da tela com a conexão bem-sucedida.                      |
| **2. Respostas às Questões com Consultas SQL**     | 50 pontos (5 por questão) | Responder corretamente às 10 questões com consultas SQL precisas e incluir os prints das consultas realizadas. |
| **3. Diagrama ER (Entidade-Relacionamento)**       | 15 pontos            | Criar um diagrama ER completo, representando tabelas e relacionamentos, com as chaves primárias e estrangeiras. |
| **4. Explicação sobre os Tipos de Relacionamento** | 15 pontos            | Explicar claramente os relacionamentos entre as tabelas e o uso das chaves estrangeiras.                    |
| **5. Organização e Apresentação do Relatório**     | 10 pontos            | Relatório bem estruturado, claro e organizado.                                                              |
| **6. Pontualidade**                                | 10 pontos            | Entrega do relatório dentro do prazo estabelecido.                                                          |
| **Total**                                          | 100 pontos           |                                               |