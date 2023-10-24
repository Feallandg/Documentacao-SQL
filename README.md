<h1 align="center"> SQL </h1>
<div class="container">
  <div class="img" align=center>
    <img align=center alt="html" width=70 height=70 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/microsoftsqlserver/microsoftsqlserver-plain.svg">
    <img align=center alt="html" width=70 height=70 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg">  
    <h5>Documentação própria para fins estudantil, utilizando conceitos, sintaxes e exemplos em Banco de Dados Relacionais(SQL)</h5>
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
 <div align="center "class="linha">__________________________________________________________________________________________________________</div>
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
  <div align="center "class="linha">__________________________________________________________________________________________________________</div>
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
</div>
