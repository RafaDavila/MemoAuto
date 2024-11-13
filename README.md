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

<h4>Criando a tabela de clientes</h4>

![image](https://github.com/user-attachments/assets/6ae513b0-04d1-463b-aeab-ab4d3d231e11)

Mesmo processo das outras tabelas.

<h2>Inserindo os dados nas tabelas</h2>

<h4>Clientes</h4>

![image](https://github.com/user-attachments/assets/5fac64e1-712f-45f9-96ca-98552f6e677d)

Após inserir os dados na tabela "clientes", é só usar o SELECT para ver os dados registrados na tabela.

![image](https://github.com/user-attachments/assets/660e45cb-02b0-4d54-9554-1bdb8705c85e)

<h4>Marcas</h4>

![image](https://github.com/user-attachments/assets/2d76c69e-1fd6-49c4-a903-87e6a0be5e67)

Mesmo processo dos clientes, mas agora com os valores "nome_da_marca" e "origem".

<h4>Iventário</h4>

![image](https://github.com/user-attachments/assets/e90ae1b6-8ba9-4c30-8d01-bc9418c8bfb2)

Agora aonde tem "marcas_id" colocar o id correspondente da marca do carro.

<h2>Criação de Usuários</h2>

Agora no PopSQL, criei a usuária "Julia" identificada por um ID genérico.

![image](https://github.com/user-attachments/assets/7fd6927c-c730-491b-ab85-a6dba27ecf3e)

Depois, criar os usuários "Pablo", que só poderá acessar o banco de dados pelo localhost, e "Márcia", que só poderá acessar o banco de dados só quando ela estiver na empresa "MemoAuto".

![image](https://github.com/user-attachments/assets/33eed81a-28e2-4636-b94e-6732c0237c1a)

<h2>Cenários Hipotéticos</h2>

Simulando alguns cenários que poderiam acontecer com uma empresa, fiz as seguintes situações:

1)Um funcionário é demitido e precisa ser deletado do banco de dados

![image](https://github.com/user-attachments/assets/6a78601d-3908-482c-ae88-c3ce2a0d8747)

2)Um funcionário perdeu ou esqueceu a senha e precisa de uma nova

![image](https://github.com/user-attachments/assets/8cb6f25c-9395-4dc1-bf79-cb3dd649e836)

Ou também, posso fazer isso pelo WorkBench:

![image](https://github.com/user-attachments/assets/4e396e94-f37c-4d8b-ab5d-bb40a6a0decd)

<h2>Adicionando privilégios para o usuário</h2>

Adicionei o acesso a "SELECT, INSERT, UPDATE, DELETE" do banco de dados para o usuário @pablolocalhost

![image](https://github.com/user-attachments/assets/f19f19f4-19ed-4ca1-8579-3ea45574bf97)

<h4>Adicionando um ADMIN</h4>

![image](https://github.com/user-attachments/assets/779a8398-bc93-4727-b986-7dde343e8853)

Usei o *.* para dizer que o usuário Pablo@localhost seja ADMIN de todos os servidores.

<h2>Consultas no banco de dados</h2>

Farei alguma consultas no banco de dados

1) Consultar os veículos disponíveis no inventário, mostrando modelo, transmissão e tipo de combustível

 ![image](https://github.com/user-attachments/assets/be0d606c-b537-4ca9-aac6-f5d362ad79eb)

2) Consultar todos os modelos da marca "Toyota":

![image](https://github.com/user-attachments/assets/a0137d9e-d947-4c3f-bf4f-7c8a9f6fb768)

3) Listar os veículos por tipo de combustível e contar quantos são de cada tipo

![image](https://github.com/user-attachments/assets/11b688b6-4d23-4138-9c91-5a8b4fdcc9fa)

4)Listar as origens das marcas no inventário e quantos modelos temos de cada país

![image](https://github.com/user-attachments/assets/4afc80cf-17e7-4847-a5ad-2f6a29668cab)

E esse foi meu projeto banco de dados "MemoAuto" ! Obrigado por chegar até aqui e continuarei com projetos e aumentando meu conhecimento.





























