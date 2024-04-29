# laboratorioai900-4
Explore um índice do Azure AI Search (UI)

1 - Criar um recurso do Azure AI Search - Lembre-se de colocar o valor como basic
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/2d8fb5a6-2f2a-4d0c-82ef-6a215014a319)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/e59598e1-1422-4c9a-a65d-c43ce65b571a)


2 - Após criado, criar um outro recurso Azure AI Services -  Sua solução de pesquisa usará esse recurso para enriquecer os dados no armazenamento de dados com insights gerados por IA.
OBS: Criar no meus resource group
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/f13c3904-cd4c-4aa0-95be-58c3ff5cb0c8)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/ac2cd91e-3445-458b-b4d0-9ddbb9d5a5b3)

3 - Criado os 2 serviços, precisaremos criar uma storage account
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/104e6bed-2973-4478-a6e7-1b2c7b49ccc0)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/5daa8782-4f1b-4064-b7eb-efb03bc874ac)

4 - Após criado, entre no recurso e vá em configurações para alterar a configuração de Permitir acesso anônimo de Blob para "Habilitado" e selecione Salvar.
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/f14f942b-7706-42b0-9938-b5499eced701)

5 - Carregar alguns arquivos para o Storage Account - No painel esquerdo Selecione Containers 
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/b64317f4-f275-432f-ae8e-02d96e9506ca)

6 - Para os próximos passo, seguiremos a documentação oficial da Microsoft. Iremos criar o container com algumas informações
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/ce8bffc0-be07-42b0-bbc7-74b3df36f29d)

7 - instalaremos uma pasta compactada das avaliações exemplos de alguns clientes - Acesse o link para instalação- https://aka.ms/mslearn-coffee-reviews

8 - Após instalar as avaliações, iremos carrega-las no nosso container que foi criado
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/a19c3da8-e694-443d-84f7-8a2dbb97756e)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/80087a48-7a14-4f57-b28e-98dcdcc0f336)

9 - Depois de armazenar os documentos, você poderá usar o Azure AI Search para extrair insights dos documentos. O portal do Azure fornece um assistente de importação de dados . Com este assistente, você pode criar automaticamente um índice e um indexador para fontes de dados suportadas. Você usará o assistente para criar um índice e importar seus documentos de pesquisa do armazenamento para o índice do Azure AI Search.
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/3dfdbdc7-a7ee-4cec-a570-dce3ce371e29)

10 - Importaremos os dador do nosso Blob, mas para isso iremos preencher alguns campos
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/04592c0f-2079-4adb-8bea-08a1ae6f8afb)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/efcdec0e-db96-465c-83e9-02af57532fc1)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/44eb4fbc-cc43-4949-b77c-384e01965f89)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/0da5715a-f343-4231-938e-a8dd8648eb53)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/756197a4-7f87-4360-b552-82a3688e780e)

11 - Após vários preenchimentos selecione Enviar para criar a fonte de dados, o conjunto de habilidades, o índice e o indexador. O indexador é executado automaticamente e executa o pipeline de indexação, que:
* Extrai os campos de metadados do documento e o conteúdo da fonte de dados.
* Executa o conjunto de habilidades cognitivas para gerar campos mais enriquecidos.
* Mapeia os campos extraídos para o índice.
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/b08a04e2-4d66-4ce8-beca-a18509d8e77b)

12 - Todo processo finalizado, hora de testar
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/8f1641b9-d031-4b94-9080-dc6b312ace87)
![image](https://github.com/JoaoP2000/laboratorioai900-4/assets/72104542/cd299d13-4a3f-4d0a-b851-3d232b6a2076)


Importante seguir o passo a passo da documentação oficial da microsoft https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html


