# MemoAuto
Banco de dados SQL de uma montadora fictícia de carros

<h2>Criando a DATABASE</h2>
Passo inicial, usando o código de criação de databases do MySQL

![image](https://github.com/user-attachments/assets/96337226-aafa-4664-87e8-95c3946ecce3)

<h2>Criando as TABLES</h2>
Primeiramente criar a tabela "Marcas" para colocar as marcas do carro:<br>
CRIANDO A ID NOT NULL, para nunca poder ser vazio, e o AUTO_INCREMENT para automaticamente criar a próxima ID.<br>

![image](https://github.com/user-attachments/assets/302321f6-9822-49cd-be81-2142b764aa3b)<br>

1)marcas_id:nome da tabela;<br>
2)INT: número inteiro;<br>
3) NOT NULL: Não pode ser vazio;<br>
4) AUTO_INCREMENT: Gera valores automaticamente para cada nova linha inserida, incrementando o último valor registrado em marcas_id;<br>
5)nome_da_marca: nome da tabela;<br>
6)VARCHAR(255): Tipo de dado para armazenar texto, com limite máximo de 255 caracteres;<br>
7)PRIMARY KEY (marcas_id): fazer a marcas_id ser minha primary key, para que seja unica em cada linha.<br>

<h4>Criando a tabela de iventário</h4>

![image](https://github.com/user-attachments/assets/2251da43-4e3c-479c-ba59-10981a1ef7eb)

1)marcas_id: Coluna de FOREIGN KEY que se relaciona com a tabela marcas. O valor nesta coluna deve existir na coluna marcas_id da tabela marcas.<br>
2)FOREIGN KEY (marcas_id) REFERENCES marcas(marcas_id): Define a coluna marcas_id como uma chave estrangeira que referencia a coluna marcas_id da tabela marcas. Isso cria um vínculo entre iventario e marcas, garantindo que qualquer valor em marcas_id na tabela iventario já exista na tabela marcas.















