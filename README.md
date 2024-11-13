# MemoAuto
Banco de dados SQL de uma montadora fictícia de carros

<h2>Criando a DATABASE</h2>
Passo inicial, usando o código de criação de databases do MySQL
![image](https://github.com/user-attachments/assets/96337226-aafa-4664-87e8-95c3946ecce3)

<h2>Criando as TABLES</h2>
Primeiramente criar a tabela "Marcas" para colocar as marcas do carro:
CRIANDO A ID NOT NULL, para nunca poder ser vazio, e o AUTO_INCREMENT para automaticamente criar a próxima ID.
![image](https://github.com/user-attachments/assets/eeda9861-55b9-4589-a368-95e3c292684c)
1)marcas_id:nome da tabela;
2)INT: número inteiro;
3) NOT NULL: Não pode ser vazio;
4) AUTO_INCREMENT: Gera valores automaticamente para cada nova linha inserida, incrementando o último valor registrado em marcas_id;
5)nome_da_marca: nome da tabela;
6)VARCHAR(255): Tipo de dado para armazenar texto, com limite máximo de 255 caracteres;
7)PRIMARY KEY (marcas_id): fazer a marcas_id ser minha primary key, para que seja unica em cada linha.
8)ALTER TABLE: alterar a tabela "marcas" e adicionar a coluna "origem".

<h4>Criando a tabela de iventário</h4>





