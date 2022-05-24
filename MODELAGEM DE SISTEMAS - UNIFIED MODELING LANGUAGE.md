###             MODELAGEM DE SISTEMAS - UNIFIED MODELING LANGUAGE

------

#### O QUE É UML?

Linguagem unificada que habilita o profissional de TI a modelar e documentar aplicações de software.

UML oferece um meio de visualizar a arquitetura de um sistema por meio de diagramas, atividades e componentes individuais do sistema, interfaces, interação entre componentes e com o mundo externo e entre outras.

- UML NÃO É UM MÉTODO DE DESENVOLVIMENTO 

- É INDEPENDENTE DE PLATAFORMA/LINGUAGEM.

- 

###  REPRESENTAÇÃO DE UM DIAGRAMA 

------

Existem duas visões distintas de um modelo de sistema, divididos em:

- Estática (ESTRUTURAL):

  > Por meio de objetos, operações, relações e atributos.

- Dinâmica (COMPORTAMENTAL):

  > Comportamento dinâmico por meio de colaboração entre objetos e mudanças de seus estados internos, mostrando o funcionamento dos sistemas. 



#### **DIAGRAMAS UML**

------

|    ESTRUTURAIS     |     COMPORTAMENTAIS      |
| :----------------: | :----------------------: |
|      classes       |       casos de uso       |
|      objetos       |        sequência         |
|      pacotes       |       comunicação        |
|    componentes     |    máquina de estados    |
|    implantação     |        atividade         |
| estrutura composta | visão geral de interação |
|       perfil       |       temporização       |



#### **DIAGRAMAS DE CLASSES UML**

------

- Descreve através de estruturas estáticas de classes o que deve estar presente em um sistema modelado.

- Permite a definição de atributos, operações (métodos)  relacionamentos entre classes.

- Define uma estrutra lógica através de uma visão estática da organização de classes.

  

**CLASSES:**

> Representação de um item do mundo real, físico ou abstrato, na forma de dados personalizados.
>
> Possuem estruturas internas chamadas de atributos e métodos.
>
> > **Atributos:** usados para armazenar dados dos objetos de uma classe. Informações sobre aquela classe do mundo real.
>
> > **Métodos:** Operações ou funções que a classe ou instância de classes vão executar. (Procedimento e função)

**EX:**

Classe: *Pessoa*

Atributos: *Altura, Nome, Peso, Idade, Sexo*

Métodos: *Andar, falar, vestir, dormir, trabalhar, estudar, correr*

Objeto da classe (Instância):

Atributos:

- Nome: Maria
- Altura: 1,60
- Idade: 45
- Peso: 57



#### **REPRESENTAÇÃO DE UMA CLASSE**

------

Uma classe é representada por um diagrama dividido em três compartimentos:

- Nome: Inclui o nome e o estereótipo da classe (Informação sobre a classe)
- Atributos: Lista de atributos da classe no formato *nome:tipo* ou *nome:tipo=valor*
- Operações: Lista de métodos da classe no formato *método(parâmetros): tipo_retorno*



#### **VISIBILIDADE DOS ATRIBUTOS/MÉTODOS**

------

| PÚBLICO       |  +   |
| ------------- | :--: |
| **PROTEGIDO** |  #   |
| **PRIVADO**   |  -   |
| **PACOTE**    |  ~   |
| **DERIVADO**  |  /   |



#### **REPRESENTAÇÃO DE UMA CLASSE**

------

| PESSOA                                                       | Nome da Classe     |
| ------------------------------------------------------------ | ------------------ |
| - nome: String <br/>- sobrenome: String <br/>- dataNasc: Date | Lista de Atributos |
| + calculaIdade(dataNasc): Int<br />+ estuda(): void          | Lista de Métodos   |

Representando acima a classe "*PESSOA*", contendo os atributos *nome, sobrenome, dataNAsc* e método *calculaIdade*.



#### ***CASOS DE USO***

-----

De acordo com Booch, Rumbaugh e Jacobson, ***"Um caso de uso especifica o comportamento de um sistema (ou parte), e é uma descrição de um conjunto de sequências de ações para produzir um resultado observável do valor de um ator"***.

- Casos de uso são usados para captar comportamentos pretendidos de um sistema, sem especificar como esse comportamento será implementado. 
- Também é possível executar uma quantidade específica de trabalho, realizando algo que seja de valor para um ator, exemplo disso é o cálculo de um resultado. 
- Casos de usos podem ter *variantes,* inclui-se parte de outros casos de uso ainda que estendam o comportamento de um caso base.
- Representam aspectos de comportamento de uma classe e modelam requisitos.

**APLICAÇÕES DOS CASOS DE USO**

-----

1. Definir Escopo - Visualizar e entender funcionalidades presentes no sistema
2. Identificar papeis - Identificar quem interage com o sistema e quais as funcionalidades da interação.
   - Os casos de uso **NÃO** são empregados para detalhar a implementação de funcionalidades.
   
   

#### **TIPOS DE CASOS DE USO**

----

1. **ASSUNTO**

- O que se trata o conjunto do determinado caso de uso.
- É uma classe descrita por um conjunto de casos de uso.
- Representa um sistema ou um subsistema.

2. **NOMES**

 - TODO caso de uso possui um nome de identificação e diferenciação dos demais casos de uso do sistema

 - Nome é uma sequência de caracteres de texto, deve ser único no pacote contido.

 - Nomes são expressões verbais ativas, que nomeiam um comportamento específico do sistema.

   EXEMPLOS DE NOMES DE CASOS DE USO:

   > - Fazer pedido
   > - Pagar Fatura
   > - Ler Sensor