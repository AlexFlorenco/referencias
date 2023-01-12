# Referência MySQL 

### Acessar MySQL
```
mysql -u root -p
```


### Listar bancos de dados
```
SHOW DATABASES;
```


### Criar banco de dados
```
CREATE DATABASE banco_de_dados;
```


### Acessar banco de dados
```
USE banco_de_dados;
```


### Criar tabela
```
CREATE TABLE nome_tabela (
    nome_coluna      tipo_de_dado    constraint,
    nome_coluna2     tipo_de_dado    constraint,
    nome_coluna3     tipo_de_dado    constraint,
    FOREIGN KEY (nome_coluna) REFERENCES outra_tabela(outra_coluna)
    );
```


###  Listar tabelas
```
SHOW TABLES;
```


### Visualizar dados da tabela
```
DESCRIBE nome_tabela;
```


### Adicionar novo campo 
```
ALTER TABLE nome_tabela ADD nome_coluna4 tipo_de_dado constraint;
```


### Adicionar uma restrição
```
ALTER TABLE nome_tabela ADD CONSTRAINT contraint (nome_coluna);
```


### Alterar o tipo de dado
```
ALTER TABLE nome_tabela MODIFY nome_coluna tipo_de_dado; 
```
> Nem sempre é permitido alterar o tipo um campo, pois pode haver perda de dados.


### Alterar nome e tipo de uma coluna
```
ALTER TABLE nome_tabela CHANGE novo_nome_coluna tipo_de_dado;
```


### Remover um campo
```
ALTER TABLE nome_tabela DROP nome_coluna;
```


### Remover uma restrição
```
ALTER TABLE nome_tabela DROP constraint;
```



