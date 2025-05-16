# 05 - Criar armazenamento de blob (5 min)

Neste exemplo vamos criar uma conta de armazenamento e trabalhar com arquivos de armazenamento de blobs.

## Tarefa 1: Criar uma conta de armazenamento

Nesta tarefa, vamos criar uma nova conta de armazenamento.

1. Acesse o portal do Azure: <a href="https://portal.azure.com" target="_blank"><span style="color: #0066cc;" color="#0066cc">https://portal.azure.com</span></a>

2. No menu **Todos os serviços**, pesquise por **Contas de Armazenamento** e clique em **+ Adicionar, + Criar ou + Nova**.

3. Na aba **Básico** da tela **Criar conta de armazenamento**, preencha as seguintes informações (substitua **xxxxx** no nome da conta por letras e números para que o nome seja único globalmente). Mantenha os demais valores padrão.

    | Configuração | Valor |
    | --- | --- |
    | Assinatura | **Mantenha o padrão fornecido** |
    | Grupo de recursos | **Criar novo grupo de recursos** |
    | Nome da conta de armazenamento | **storageaccountxxxxx** |
    | Localização | **(EUA) Leste dos EUA** |
    | Desempenho | **Padrão** |
    | Redundância | **Armazenamento localmente redundante (LRS)** |

    **Observação**: Lembre-se de alterar o **xxxxx** para garantir um nome único da conta.

4. Clique em **Revisar + Criar** para revisar as configurações e permitir que o Azure valide.

5. Após a validação, clique em **Criar**. Aguarde até que a notificação de criação seja exibida.

6. Na página inicial, pesquise por **Contas de Armazenamento** e verifique se sua nova conta aparece na lista.

## Tarefa 2: Trabalhar com blob storage

Nesta tarefa, criaremos um contêiner de blobs e faremos upload de um arquivo blob.

1. Clique no nome da nova conta de armazenamento, vá até a seção **Armazenamento de dados** no menu à esquerda e clique em **Contêineres**.

2. Clique em **+ Contêiner** e preencha as informações. Use os ícones de informação para saber mais. Em seguida, clique em **Criar**.

    | Configuração | Valor |
    | --- | --- |
    | Nome | **container1** |
    | Nível de acesso público | **Privado (sem acesso anônimo)** |

3. Em outra janela do navegador, pesquise no **Bing** por uma imagem de flor. Clique com o botão direito na imagem e salve no seu computador/VM.

4. No portal, clique em **container1** e depois em **Upload**.

5. Localize e selecione o arquivo de imagem salvo. Em seguida, clique em **Upload**.

6. Clique na seta **Avançado**, revise as opções (mantendo os valores padrão) e clique em **Upload**.

    **Observação**: Você pode fazer upload de quantos blobs quiser. Novos blobs aparecerão listados no contêiner.

7. Após o upload, clique com o botão direito no arquivo e explore as opções: Visualizar/editar, Baixar, Propriedades e Excluir.

8. Se tiver tempo, explore as opções para Arquivos, Tabelas e Filas.

## Tarefa 3: Monitorar a conta de armazenamento

1. Volte para a tela da conta de armazenamento e clique em **Diagnosticar e resolver problemas**.

2. Explore os problemas mais comuns de armazenamento. Note que há vários assistentes de solução de problemas disponíveis.

3. Ainda na conta de armazenamento, vá até a seção **Monitoramento** e clique em **Insights**. Observe as informações sobre Falhas, Desempenho, Disponibilidade e Capacidade. Seus dados podem variar.

**Observação**: Para evitar custos adicionais, você pode remover o grupo de recursos.

* Pesquise por **Grupos de recursos**, clique no seu grupo e depois em **Excluir grupo de recursos**.
* Confirme o nome e clique em **Excluir**. Acompanhe o andamento em **Notificações**.
