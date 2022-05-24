##                           MODELAGEM DE DADOS

1. **INTRODUÇÃO AO BANCO DE DADOS**

   Tendo em vista que, dados são meios que podem ser registrados ou armazenados em algum local específico. 

   EX¹: agenda telefônica - Tanto em agendas físicas ou virtuais, podem ser armazenados dados (nomes e telefones). Tudo que é possível ser armazenado, é um dado. 

   E o banco de dados nada mais é do que a coleção de dados relacionados e armazenados em algum meio/ambiente/sistema. 

   Quando falamos de Banco de Dados, temos o entendimento de que:

   - Representação baseada em um aspecto presente do mundo real (Orientada a objetos)
   - A coleção de dados é logicamente coerente
   - É projetado e construído para receber dados de finalidades específicas
   - Um banco de dados pode ter qualquer tamanho, desde uma tabela simples com poucos dados armazenados, até um servidor de larga escala que atende uma empresa multinacional. 

   <br>

   2- **DADOS ≠ INFORMAÇÃO**

   Conceitos totalmente distintos, mas relacionados.

   - **Dados:** Fatos em uma forma primária, podendo ser armazenado em qualquer meio.

     ex: CPF, Nome, Data, Altura, Peso, Cor.

     

   - **Informações:**** Fatos organizados com intuito de produzir algum significado -> Dados quando colocados em contexto.

     ex: Lista de clientes cadastrados com número do celular ou CPF.

   <br>

   3- **SGBD - SISTEMA DE GERENCIAMENTO DE BANCO DE DADOS**

      É uma coleção de softwares que permite a manuntenção e criação de um ou mais banco de dados. 

      - Usados em tarefas de definição, construção, manipulação e compartilhamento entre usuários e aplicações.
      - Proteção e segurança dos dados contra acesso e alterações sem autorização.
      - Pode ser mantido por um longo período
      - Existem diversos sistemas de gerenciamento de banco de dados disponíveis do tipo comercial e software livre.

      **Exemplos de SGBDs mais populares atualmente**

      - Oracle Database

      - Microsoft SQL Server

      - MySQL Server

      - IBM DB2

      - SAP Sybase

      - MongoDB

      - Teradata

      - PostgreSQL

      - SQLite

        
<br>
        

**4 - TIPOS DE BANCO DE DADOS.**<br>
  **4.1 - HIERÁRQUICO:** 

  

- Os dados são organizados de forma hierárquica por meio de interconexões e ligações.

- Esse modelo é um diagrama de estrutura em árvore.

- Uma ligação é representada pela relação entre dois tipos de registros: pai e filho.

- Acesso aos dados de forma unidirecional, a partir do pai ao filho. 
   
   
   ![Diferença entre modelo de dados hierárquico, de rede e relacional – Acervo  Lima](https://media.geeksforgeeks.org/wp-content/uploads/20200727113000/network.png)
   
   
<br>
   ​	4.2 - MODELO EM REDE
   
   - Os dados são organizados em tipos e ligações entre dois registros, não de forma hierárquica. 
   - Tanto o esquema quanto ocorrencias de dados são visualizados como um grafo direcionado
   
   
   
   ![Blog de Dados | Just another WordPress.com site](http://blogrdi.files.wordpress.com/2011/08/intro-bd_html_21d904ca.gif)
   
   
<br> 
   ​	4.3 - RELACIONAL (Muito importante)
   
   - Os dados são separados em entidades, conforme o tema abordado e registrados como atributos dessas entidades.
   - No modelo relacional, os dados são organizados em tabelas (relações) bidimensionais.
   - As entidades se relacionam entre si, permitindo que os dados sejam armazenados e recuperados de forma rápida e segura. 
   
   
   
   ![img](https://web.fe.up.pt/~ssn/disciplinas/cdi/bases-de-dados/er_exemplo.png)
   
   
 <br> 
   
   4.4 - **OBJETO-RELACIONAL** (BDOR ou SGBDRO)
   
   - Sistema de gerenciamento de banco de dados, semelhante a um banco de dados relacional, mas orientado a objetos.
   
     > Objetos, classes e herança suportados diretamente nos esquemas do banco de dados. 
   
   - Geralmente é usada para permitir o armazenamento de dados complexos de forma mais simples. 
   
   - Objetivo de verificar a performance de consultas em sistemas web que processam atributos complexos de dados.
   
   - Composto por coleções de objetos ou relações que armazenam dados
   
     > **Exemplo de utilização:** 
     
     > - Armazenar dados de clientes de uma loja de roupas.
     
     > Pode-se criar tabelas que armazenam diferentes conjuntos de dados relacionados a cada cliente, como dados pessoais, endereço, contatos, dados de compras (financeiro) e outras, de forma que não haja redundancia dos dados e garanta a integridade dos mesmos.
   
   
   
   4.5 - **NÃO-RELACIONAL (NoSQL)**
   
   - Projetados para análise de dados semiestruturados. 
   
   - Possui esquemas flexíveis para a criação de aplicativos modernos, possui facilidade de desenvolvimento, funcionalidade e performance em escala. 
   
   - Ideais para dispositivos móveis, Web e jogos, onde há exigencia de bancos de dados flexíveis, escaláveis, de alta performance e altamente funcionais.
   
     

​		**5. CRIAÇÃO DE BANCOS DE DADOS**

​	Os passos do processo de criação de banco de dados segue este raciocínio:

 1. Especificação e Análise de Requisitos
   - Onde os requisitos são documentados e analisados

2. **Projeto Conceitual**
   - Baseado nos requisitos

3. **Projeto Lógico**

   - Expresso em um modelo de dados, como o relacional

4. **Projeto Físico**

   - Especificações para garantir amarzenamento e acesso ao banco de dados
   - Banco de dados é implementado, alimentado com dados e reais e mantido

   

​		**6. ARQUITETURA DE UM SISTEMA DE BANCO DE DADOS**

​		*Cliente-servidor* é a arquitetura básica de um sistema de banco de dados atual, onde o sistema é 		distribuído entre dois tipos de componentes, o cliente e o servidor. 

> **Cliente:** 
>
> Executado em uma estação de trabalho ou computador pessoal.
>
> **Servidor:** 
>
> Onde ficam armazenados os dados, com módulos de acesso, consulta e demais funções.

​	

​		**7. LINGUAGEM DE BANCO DE DADOS**

- DDL (Data Definition Language/ Linguagem de Definição de Dados)

>  Utilizada pelos projetistas de bancos de dados e pelos DBAs (Database Administrators / Administradores de Bancos de Dados) para definir o esquema conceitual de um banco.

- DML – Data Manipulation Language (Linguagem de Manipulação de Dados)

  >Torna possível a manipulação do banco de dados e permite a inserção, alteração, exclusão ou recuperação dos dados.

- DQL (Data Query Language / Linguagem de Consulta de Dados)

  >São utilizados comandos para efetuar consultas e resgatar informações armazenadas em um Banco de Dados (BD)

- DCL (Data Control Language / Linguagem de Controle de Dados)

  > Atribui privilégios de acesso em um banco de dados aos usuários.

​	**OBS:** Essas linguagens não são tratadas como linguagens distintas nos SGBDs atuais, mas é utilizada uma linguagem integrada para as definições e manipulação dos dados.

**IMPORTANTE:** 

   **SQL** (Structured Query Language / Linguagem de Consulta Estruturada) 

É um exemplo típico de linguagem padrão utilizada na criação e manipulação de dados em banco de dados relacionais. 

**Exemplo de código na linguagem SQL:**

> ```
> SELECT CODIGO, NOME FROM CLIENTES
> WHERE CODIGO = 10
> SELECT CODIGO, NOME FROM CLIENTES
> WHERE UF = ‘RJ’
> SELECT CODIGO, NOME FROM CLIENTES
> WHERE CODIGO >= 100 AND CODIGO <= 500
> SELECT CODIGO, NOME FROM CLIENTES
> WHERE UF = ‘PA’ OR UF = ‘SP’
> ```

8. **CRIAR UM BANCO DE DADOS - COMANDO SQL (ALGUNS EXEMPLOS)**

​	**8.1 - Criando um Banco de Dados**

​	Para criar um novo banco de dados, é inserido o comando *CREATE DATABASE*, seguido do nome que queremos dar ao banco. Exemplo: para criar um novo banco de dados de nome "Escola" usamos o comando a seguir:

>```
>CREATE DATABASE escola;
>```

​	Após criar o banco, executamos o comando *USE* para torná-lo o banco atual:

> ```
> USE escola;
> ```

​		**8.2 - Exemplo de criação de uma Tabela**

​	Para criação de Tabelas em banco de dados, usamos a declaração *CREATE TABLE.*

​	Sintaxe:

> ```
> CREATE TABLE nome_tabela (
>  coluna1 tipo_dados constraint,
>  coluna2 tipo_dados constraint,
>  ...
>  colunaN tipo_dados constraint
> );
> ```

Foram apenas alguns exemplos de códigos que serão mais aprofundados no decorrer dos estudos. 


9 - MODELAGEM DE DADOS

- São usadas técnicas específicas de modelagem no processo de criação de modelo de Dados para um sistema de informação. Há um processo de levantamento, análise, categorização e exploração de todos os dados e tipos de informações a serem utilizadas em uma aplicação.

- Processo de definição e análise de requisitos de dados para que seja viável processar negócios com sistemas informatizados em organizações.

## 
