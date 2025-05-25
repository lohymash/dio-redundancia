1. Configuração do Ambiente Azure
Criar um Resource Group na Azure para agrupar todos os recursos

2. Configuração do Integration Runtime
No Azure Data Factory:

clique em novo

escolha o modelo que quer, neste caso, self-hosted
![image](https://github.com/user-attachments/assets/bc317dd4-305a-451d-babe-23418eb40fc9)
![image](https://github.com/user-attachments/assets/9de57435-b0fb-4037-9b31-d48f8836c59c)

configure-o e crie
![image](https://github.com/user-attachments/assets/8b9319b8-0783-4b39-ae49-33f8106b4a61)
![image](https://github.com/user-attachments/assets/fd244285-84f2-419c-9d6e-edbaab5ac86a)

4. Criação de Linked Services
Linked Service para SQL Server on-premises:
![image](https://github.com/user-attachments/assets/c4f9f777-c86f-4d98-9638-2154bd33ee83)
crie o serviço de SQL e selecione o Integration Runtime anteriormente criado para se conectar
![image](https://github.com/user-attachments/assets/0a626f47-6c2c-47f3-b6ec-3fd549b96f64)

não irei prosseguir com o setup, pois, meu computador não tem muita capacidade computacional...
porém, após isso você conseguirá linkar o self-hosted usando a Key dada após a criação do integration runtime
![image](https://github.com/user-attachments/assets/550a24a3-eb01-4e68-9ffe-432bd3a4f1e9)

5 - pipelines
![image](https://github.com/user-attachments/assets/ff98c977-378d-4ba2-97dd-a2a7e725dfee)
crie o pipeline no botão de +
![image](https://github.com/user-attachments/assets/0141b2a9-cf15-4817-a8d1-4bcfc03cdfb0)
arraste o Copy data de atividades para a telinha
![image](https://github.com/user-attachments/assets/bc10a8f7-39bc-4793-b2d7-91232875b8eb)
e aqui nesta tela aonde você passa todos os parametros, porém, não consegui realizar esta atividade pela falta de poder computacional do meu dispostivo
![image](https://github.com/user-attachments/assets/7f62ad87-c2c8-4763-89c9-eddb08770227)

