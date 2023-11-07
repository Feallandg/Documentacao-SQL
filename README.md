<h1 align="center"> SQL </h1>
<div class="container">
  <div class="img" align=center>
    <img align=center alt="html" width=70 height=70 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/microsoftsqlserver/microsoftsqlserver-plain.svg">
    <img align=center alt="html" width=70 height=70 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg">  
    <h5>Documentação própria para fins estudantil, utilizando conceitos, sintaxes e exemplos em Banco de Dados Relacionais(SQL)</h5>
    <p align="center"><img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge"/></p>
  </div>
  <div class="OqE">
    <h2>◾ O que é SQL?</h2>
    <p>▪️ Linguagem de consulta Estruturada, permite acessar e manipular dados. Tornou-se padrao em 86 pela ANSI(eua) e internacionalmente em  87 pela ISO.</p>
    <h3>◾ O que o sql pode fazer?</h3>
    <p>▪️ Consultas em um BdD, criar e recuperar dados, Inserir registros e atualiza-los ou excluir-los;</p>
    <p>▪️ Pode criar tabelas, procedimentos e exibições e definir permissões dentro de um BdD;</p>
    <h3>◾ RDBMS</h3>
    <p>▪️  Sistema de Gerenciamento de Banco de Dados Relacional.</p>
    <p>▪️ E a base do sql e todos os sistemas, os dados são armazenados em objetos de banco de dados chamado tabelas. uma tabela e uma coleção de entrada de dados relacionadas e consiste em colunas e linhas.</p>
    <p align="center">
     <img alt="rdbms" width=350 height=250 src="https://3.bp.blogspot.com/--vWgzq6KD7U/WgNzgvTG7lI/AAAAAAAAANc/4BDJojntaaQT_5q-do0hF7bxaYqoUdzywCPcBGAYYCw/s1600/rdbms_example%2B%25281%2529.jpg" />
    </p>
  </div>
 <div align="center" class="linha">__________________________________________________________________________________________________________</div>
  <div class="Comandos">
    <div class="select">
     <h3>SELECT</h3>
     <p>▪️ Extra-e dados de um banco de dados.<br> ▪️Sintaxe:<br>
 SELECT column1, column2, ...<br>
 FROM table_name;</p>
   <h4>Select Distinct</h4>
     <p>▪️ Seleciona apenas um único dado, mesmo que se repita, ele só irá mostrar um. Ex.: Se um BdD tiver 3 "alemanha", ele só irá mostrar apenas uma "alemanha".<br> ▪️Sintaxe:<br>
 SELECT DISTINCT column1, column2, ...<br>
 FROM table_name;</p>
   <h4>Select Top</h4>
     <p>▪️ Quando você seleciona a quantidade específica de dados que ira aparecer.<br> ▪️Sintaxe:<br>
SELECT TOP 3 * FROM Customers;</p>
  </div>   
  </div>
  <div align="center"class="linha">__________________________________________________________________________________________________________</div>
  <div class="where">
   <h3>WHERE</h3>
     <p>▪️ Utilizado para filtrar um dado do BdD. "AND" utilizado com o where, vai adicionar mais uma condição.<br> ▪️Sintaxe:<br>
 SELECT column1, column2, ...<br>
 FROM table_name<br>
 WHERE condition1 AND condition2 AND condition3 ...;
  <h4>OR</h4>
     <p>▪️ Você adiciona +1 condição com where.<br> ▪️Sintaxe:<br>
 SELECT column1, column2, ...<br>
 FROM table_name<br>
 WHERE condition1 OR condition2 OR condition3 ...
  <h4>NOT</h4>
     <p>▪️ Você usa qnd nao quer que tal resultado apareça.<br> ▪️Sintaxe:<br>
 SELECT column1, column2, ...<br>
 FROM table_name<br>
 WHERE NOT condition;
  <h4>LIKE</h4>
     <p>▪️Usado com where para procurar determinada palavra na tabela usado com %(Varios caracteres)  ou _(um caract).<br> ▪️Sintaxe:<br>
  SELECT * FROM Customers<br>
 WHERE City LIKE 's%';
       
  <h4>IN</h4>
     <p>▪️Parecido com o OR, mas nesse caso vc requer as condições da amostra de tabela. <br> ▪️Sintaxe:<br>
 SELECT * FROM Customers<br>
 WHERE City IN ('Paris','London');
  </div>
  <div align="center"class="linha">__________________________________________________________________________________________________________</div>
  <div class="update">
    <h3>UPDATE</h3>
     <p>▪️ Atualiza dados em um BdD;<br> ▪️Sintaxe:<br>
 UPDATE table_name<br>
 SET column1 = value1, column2 = value2, ...<br>
 WHERE condition;
 <h4>INSERT INTO</h4>
     <p>▪️Insere novos dados em um BdD; <br> ▪️Sintaxe:<br>
 INSERT INTO table_name (column1, column2, column3, ...)<br>
 VALUES (value1, value2, value3, ...);
  <h4>ORDER By</h4>
    <p>Usado para ordernar dados do BdD,  ASC: Crescente, DESC: Decrescente;<br>▪️Sintaxe:<br>
    SELECT column1, column2, ...
    FROM table_name
    ORDER BY column1, column2, ... ASC|DESC;</p>
    <h4>MIN. & MAX.</h4>
    <p>Quando você atribue o max. e o min. do dados selecionados para preços.<br>▪️Sintaxe:<br>
    SELECT MIN/MAX(column_name)<br>
    FROM table_name<br>
    WHERE condition; </p>
    <h4>COUNT</h4>
    <p>Retorna quantos dados existentes no BdD requerido. AVG ele retornará o valor médio de uma tabela.<br>
▪️Sintaxe:<br>
 SELECT COUNT(column_name)
 FROM table_name<br>
 WHERE condition;</p>
    <h4>SUM</h4>
    <p>Retorna o total de sumário de númericos da coluna;<br>
 ▪️Sintaxe:<br>
 SELECT SUM(column_name)<br>
 FROM table_name<br>
 WHERE condition;</p>
    <h4>AVG</h4>
    <p>Retorna o valor médio da tabela;<br>
 ▪️Sintaxe:<br>
 SELECT AVG(Price)<br>
 FROM Products;</p>
    <h4>BETWEEN</h4>
    <p>Uma condição que pede valores dentro de um intervalo, podendo ser txt, números e afins;<br>
 ▪️Sintaxe:<br>
 SELECT column_name(s)<br>
 FROM table_name<br>
 WHERE column_name BETWEEN value1 AND value2;</p>
    <h4>ALIASES</h4>
    <p>Usado para dar um nome temporário a uma tabela;<br>
 ▪️Sintaxe:<br>
 SELECT CustomerID AS ID<br>
 FROM Customers;</p>
  </div>
  <div align="center"class="linha">__________________________________________________________________________________________________________</div>
  <div class='JOINS'>
    <h3>JOINS</h3>
    <p> Usado para combinar linhas de duas ou mais tabelas;</p>
    <p align="center">
     <img alt="rdbms" width=370 height=270 src="https://learnsql.com/blog/learn-and-practice-sql-joins/2.png" />
    </p>
    <h4>INNER JOIN</h4>
    <p> Seleciona arquivos em ambas tabelas selecionadas;<br>
  ▪️Sintaxe:<br>
   SELECT column_name(s)<br>
   FROM table1<br>
   INNER JOIN table2<br>
   ON table1.column_name = table2.column_name;</p>
    <h4>LEFT JOIN</h4>
    <p> Junção de 2 tabelas interessado de ajuntar dados das 2 tabelas.<br>
    ▪️Sintaxe:<br>
     SELECT column_name(s)<br>
     FROM table1<br>
     LEFT JOIN table2<br>
     ON table1.column_name = table2.column_name;</p>
   <h4>RIGHT JOIN</h4>
    <p>Vice-versa do left join, seleciona pelo lado direito(2) da ocasião;<br>
    ▪️Sintaxe:<br>
     SELECT column_name(s)<br>
     FROM table1<br>
     RIGHT JOIN table2<br>
     ON table1.column_name = table2.column_name;</p>
    <h4>FULL JOIN</h4>
    <p>Irá selecionar os dois lados(1&2), retornando o msm atributo requerido;<br>
▪️Sintaxe:<br>
 SELECT column_name(s)<br>
 FROM table1<br>
 FULL OUTER JOIN table2<br>
 ON table1.column_name = table2.column_name<br>
 WHERE condition; </p>
  </div>
  <div align="center"class="linha">__________________________________________________________________________________________________________</div>
  <div class='UNION'>
    <h3>UNION</h3>
    <p>Um operador que combina conjuntos do Select, esse operador seleciona apenas valores distintos por padrão. Para permitir valores duplicados, use "UNION ALL";<br>
▪️ Sintaxe:<br>
 SELECT column_name(s) FROM table1<br>
 UNION<br>
 SELECT column_name(s) FROM table2;
</p>
    <h4>GROUP BY</h4>
    <p>Ele agrupa dados em linhas;<br>
▪️ Sintaxe: <br>
 SELECT column_name(s)<br>
 FROM table_name<br>
 WHERE condition<br>
 GROUP BY column_name(s)<br>
 ORDER BY column_name(s);</p>
    <h4>SELECT INTO</h4>
    <p> Seleciona dados de uma tabela para copiar, usando o IN para alocar em outro banco;<br>
▪️ Sintaxe: <br>
 SELECT *<br>
 INTO newtable [IN externaldb]<br>
 FROM oldtable<br>
 WHERE condition;<br></p>
    <h4>CASE</h4>
    <p>Se relaciona muito com um IF/Else de uma línguagem, utilizado para tratamento de uma consulta. Utilizando "when" para uma condição, e para trazer o resultado, utilizamos then; <br>
▪️ Sintaxe: <br>
 SELECT *<br>
 INTO newtable [IN externaldb]<br>
 FROM oldtable<br>
 WHERE condition;<br></p>
  </div>
  <div align="center"class="linha">__________________________________________________________________________________________________________</div>
  <div calss='SQL DTBSE'></div>
  <h4>Como criar um banco de dados ou exclui-lo?</h4>
  <p>"CREATE DATABASE ..." & "DROP DATABASE ...", você exclue;<br>
▪️ Sintaxe: <br> CREATE DATABASE databasename; & DROP DATABASE databasename;<br></p>
   <h4>Como atualizar um banco de dados?</h4>
  <p>"BACKUP DATABASE ...", Você atualiza o db, utilizando to disk e with.<br>
▪️ Sintaxe: <br>
 BACKUP DATABASE databasename<br>
 TO DISK = 'filepath';</p>
   <h4>Como criar uma tabela e exclui-la?</h4>
  <p>"CREATE TABLE ..." E "DROP TABLE", Exclue;<br>
▪️ Sintaxe: <br>
 CREATE TABLE table_name (<br>
    column1 datatype,<br>
    column2 datatype,<br>
    column3 datatype,<br>
   ....
 );</p>
   <h4>Como alterar algo na tabela?</h4>
  <p>"ALTER TABLE ..." Usado para criar, deletar e modificar colunas já existentes;<br>
▪️ Sintaxe: <br>
 ALTER TABLE table_name<br>
 ADD column_name datatype;<br>
</p>
   <h4>Como especificar meus dados em uma tabela?</h4>
  <p>'column1 datatype "CONSTRAINT"', usado para especificar caminhos dos dados em uma tabela.<br>
▪️ Sintaxe: <br>
 CREATE TABLE table_name (<br>
    column1 datatype constraint,<br>
    column2 datatype constraint,<br>
    column3 datatype constraint,<br>
    ....
 );</p>
   <h4>O que é NOT NULL?</h4>
  <p>"NOT NULL", Ele trás que os valores null não serão aceitados para a tabela.<br>
▪️ Sintaxe: <br>
 CREATE TABLE Persons (<br>
    ID int NOT NULL,<br>
    LastName varchar(255) NOT NULL,<br>
    FirstName varchar(255) NOT NULL,<br>
    Age int
 );</p>
  <div align="center"class="linha">__________________________________________________________________________________________________________</div>
  <div class='KEY'>
    <h4>UNIQUE</h4>
    <p>Garante que todos os valores de uma coluna seja diferente. Promovendo uma exclusividade para as colunas.<br>
▪️ Sintaxe: <br>
 CREATE TABLE Persons (<br>
    ID int NOT NULL UNIQUE,<br>
    LastName varchar(255) NOT NULL,<br>
    FirstName varchar(255),<br>
    Age int
 );</p>
    <h4>PRIMARY KEY(chave primária)</h4>
    <p>A chave primaria E um indentificador unico da tabela. Sendo unico, mas nao nulo. Todo registro de tabela só deverar ter apenas uma chave primaria. <br>
▪️ Sintaxe: <br>
 CREATE TABLE Persons (<br>
    ID int NOT NULL UNIQUE,<br>
    LastName varchar(255) NOT NULL,<br>
    FirstName varchar(255),<br>
    Age int
 );
</p>
    <h4>FOREIGN KEY(chave estrangeira)</h4>
    <p>Foreign Key ou chave estrangeira, elas buscam as relações entre tabelas. Podendo ser um referência de uma tabela "x" para uma chave primaria da tabela "y", Podendo ser nula.<br>
▪️ Sintaxe: <br>
 CREATE TABLE Persons (<br>
    ID int NOT NULL UNIQUE,<br>
    LastName varchar(255) NOT NULL,<br>
    FirstName varchar(255),<br>
    Age int
 );</p>
    <h4>CHECK</h4>
    <p>Usado para uma limitação de intervalos de valores dentro de uma tabela.<br>
▪️ Sintaxe: <br>
 CREATE TABLE Persons (<br>
    ID int NOT NULL,<br>
    LastName varchar(255) NOT NULL,<br>
    FirstName varchar(255),<br>
    Age int CHECK (Age>=18)<br>
 );</p>
  </div>
  <div align center class='agradecimentos'>
    <h4>Se você chegou até aqui, desde já te agradeço pela vizualização!😁 </h4>
  </div>
</div>
 
