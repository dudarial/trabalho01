# TRABALHO 01: REMEDMEX
Trabalho desenvolvido durante a disciplina de Banco de Dados do Integrado.

# Sumário

### 1.COMPONENTES<br>
Integrantes do grupo<br
laira: lairaarruda@gmail.com<br>
maria eduarda: dudah.jbraga@gmail.com<br>
...

### 2.INTRODUÇÃO E MOTIVAÇAO<br>
Este documento contém a especificação do projeto do banco de dados <remedmax> 
<br>e motivação da escolha realizada. <br>
 
 > O sistema da empresa "remedmex" tem como intuito gerenciar a saúde das pessoas. O usuário informa qual o diagnóstico obtido pelo médico, o aplicativo armazena em seu banco de dados, e analisa a ocorrência da doença na região. Se a ocôrrencia for frequente na região, o aplicativo informa um alerta de possível epidemia. Juntamente a isso, o usuário pode informar qual medicação está usando, e o dispositivo, além de mandar um alerta nos horários das medicações, sugestões de genéricos e/ou outros remédios que podem ser úteis, indicando um medicamento de acordo com as especificações de cada pessoa. O objetivo é que o software ajude a diminuir os casos de pessoas que têm seus estados de saúde agravados por não terem buscado auxílio médico antes. Nesse quesito, o aplicativo indicaria, caso fosse necessário, que o usúario buscasse atendimento médico, evitando tais enfermidades.

### 3.MINI-MUNDO Novo<br>

Descrever o mini-mundo! (Não deve ser maior do que 30 linhas) <br>
Entrevista com o usuário e identificação dos requisitos.<br>
Descrição textual das regras de negócio definidas como um  subconjunto do mundo real 
cujos elementos são propriedades que desejamos incluir, processar, armazenar, 
gerenciar, atualizar, e que descrevem a proposta/solução a ser desenvolvida.

> O sistema proposto para o "remedmex" terá salvo em seu banco e dados as informações dos usuários para <b>cadastro</b>, que ficarão registradas em cada conta, assim como seu login e senha. Juntamente a essas informações, o usuário também irá informar outros dados, como por exemplo data de nascimento, sexo, peso, altura, email e, principalmente, o CPF. Contudo, também deverá informar dados de sua saúde, como: Convênio, número da carteirinha, número do sus, tipo sanguíneo, se faz uso de alguma medicação recorrente, se possui alguma doença crônica e/ou alguma alergia. Para ter controle sobre as regiões epidêmicas, solicita-se juntamente, informações sobre a localidade do usuário, tais como endereço, CEP, bairro onde mora, cidade, estado, número da residência e complemento, caso houver. Caso o paciente faça uso de alguma medicação, o aplicativo notificará nos respectivos horários desta. O sistema terá que armazenar no banco de dados os sintomas de várias doenças, se há ocorrência de epidemias na região e asssociar os sintomas do usuário a essas informações locais.

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser desenvolvidas. O princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas e/ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Arquivo PDF do Protótipo Balsamiq feito para Empresa Devcom]
(https://github.com/remedmax/trabalho01/blob/master/arquivos/remedmex.pdf?raw=true "Empresa Remedmex")


#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    a) O sistema proposto poderá fornecer quais tipos de relatórios e informaçes? 
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto!
    
> A remedemex precisa inicialmente dos seguintes relatórios:
* Relatório de cadastro que informe as seguintes informações sobre o paciente: nome e sobrenome, email, uma senha acessível, idade, sexo, peso e altura.
* Relatório de consulta que informará: especialização e sugestão de médicos, consultas marcadas, hospitais e horários disponíveis.
* Relatório de medicação que indicará: remédios e horário específico.
* Relatório com dados gerais para registrar a consulta que informará: o médico, hospital, data, diagnóstico e a receita.
* Relatório que armazenará uma diagnóstico, localizará o local e registrará: locais com epidemias.
 
 
#### 4.2 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
    
 ![Exemplo de Tabela de dados do Programa Remedmex](https://github.com/remedmax/trabalho01/blob/master/arquivos/DadosProgramaRemedmexATT%20(1).xlsx?raw=true "Tabela - Programa Remedmex")
 
>## Marco de Entrega 01 em: (24/03/2018)<br>

### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
        * Para nosso prótótipo limitaremos o modelo conceitual nas 5 principais entidades do escopo
        * O protótipo deve possui no mínimo duas relações N para N
        * o mínimo de entidades do modelo conceitual será igual a 5
        
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/md_conceitualatt2.png?raw=true "Modelo Conceitual")



    B) NOTACAO UML (Caso esteja fazendo a disciplina de analise)
    C) QUALIDADE 
        Garantir que a semântica dos atributos seja clara no esquema
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas.
        
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]
## Marco de Entrega 01 em: (20/04/2018)<br>
#### 5.2 DECISÕES DE PROJETO
    [atributo]: [descrição da decisão]
    
    [Medicação]: Optamos por não especificar o campo medicação, visto que exige muitas tabelas e dados, decidimos fazê-los depois.
    [Hospital - localidade]: Decidimos incluir as relações de localidade do hospital posteriormente, pois o trabalho já possui muitas extensões.

#### 5.3 DESCRIÇÃO DOS DADOS 
    [objeto]: [descrição do objeto]
    
    EXEMPLO:
    CLIENTE: Tabela que armazena as informações relativas ao cliente<br>
    CPF: campo que armazena o número de Cadastro de Pessoa Física para cada cliente da empresa.<br>

>## Marco de Entrega 01 em: (12/05/2018)<br>
### 6	MODELO LÓGICO<br>
        a) inclusão do modelo lógico do banco de dados:
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/L%C3%B3gico_1.png?raw=true "Modelo Lógico")
   
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)

### 7	MODELO FÍSICO<br>
        a) inclusão das instruções de criacão das estruturas DDL 
        (criação de tabelas, alterações, etc..)         
    CREATE TABLE PESSOA (
     CPF varchar(20) PRIMARY KEY,
     nome varchar(30),
     email varchar(45),
     sexo char,
     altura int,
     dt_nascimento date,
     peso int,
     n_carteirinha varchar(20),
     n_sus varchar(20),
     alergias varchar(30),
     doencas_cronicas varchar(30),
     tp_sanguineo char(3),
     CEP varchar(20),
     complemento varchar(20),
     convenio varchar(20),
     n_residencia int,
     FK_BAIRRO_cod_bairro int
     );

    CREATE TABLE CONSULTA (
    dt_consulta date,
    hora time,
    status varchar(30),
    cod_consulta int PRIMARY KEY,
    FK_PESSOA_CPF varchar(20),
    FK_HOSPITAL_cod_hospital int,
    FK_DIAGNÓSTICO_cod_diag int );

    CREATE TABLE HOSPITAL (
    nome varchar(30),
    cod_hospital int PRIMARY KEY );

    CREATE TABLE DIAGNÓSTICO (
    cod_diag int PRIMARY KEY,
    receita varchar(30),
    doença varchar(10) );

    CREATE TABLE BAIRRO (
    nome varchar(30),
    cod_bairro int PRIMARY KEY,
    FK_CIDADE_cod_cidade int );

    CREATE TABLE CIDADE (
    nome varchar(30),
    cod_cidade int PRIMARY KEY,
    FK_ESTADO_cod_estado int );

    CREATE TABLE ESTADO (
    nome varchar(30),
    cod_estado int PRIMARY KEY);

    CREATE TABLE Trabalha (
    FK_HOSPITAL_cod_hospital int,
    FK_PESSOA_CPF varchar(20));
 
    ALTER TABLE PESSOA ADD CONSTRAINT FK_PESSOA_1
     FOREIGN KEY (FK_BAIRRO_cod_bairro)
     REFERENCES BAIRRO (cod_bairro)
     ON DELETE CASCADE ON UPDATE CASCADE;
 
    ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_1
     FOREIGN KEY (FK_PESSOA_CPF, FK_PESSOA_CPF_)
     REFERENCES PESSOA (CPF, CPF)
     ON DELETE CASCADE ON UPDATE CASCADE;
 
    ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_2
     FOREIGN KEY (FK_HOSPITAL_cod_hospital)
     REFERENCES HOSPITAL (cod_hospital)
     ON DELETE CASCADE ON UPDATE CASCADE;
 
    ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_3
     FOREIGN KEY (FK_DIAGNÓSTICO_cod_diag)
     REFERENCES DIAGNÓSTICO (cod_diag)
     ON DELETE CASCADE ON UPDATE CASCADE;
 
    ALTER TABLE BAIRRO ADD CONSTRAINT FK_BAIRRO_1
     FOREIGN KEY (FK_CIDADE_cod_cidade)
     REFERENCES CIDADE (cod_cidade)
     ON DELETE RESTRICT ON UPDATE RESTRICT;
 
    ALTER TABLE CIDADE ADD CONSTRAINT FK_CIDADE_1
     FOREIGN KEY (FK_ESTADO_cod_estado)
     REFERENCES ESTADO (cod_estado)
     ON DELETE RESTRICT ON UPDATE RESTRICT;
 
    ALTER TABLE Trabalha ADD CONSTRAINT FK_Trabalha_0
     FOREIGN KEY (FK_HOSPITAL_cod_hospital)
     REFERENCES HOSPITAL (cod_hospital)
     ON DELETE SET NULL ON UPDATE CASCADE;
 
    ALTER TABLE Trabalha ADD CONSTRAINT FK_Trabalha_1
     FOREIGN KEY (FK_PESSOA_CPF)
     REFERENCES PESSOA (CPF)
     ON DELETE SET NULL ON UPDATE CASCADE;

         
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físic
        b) formato .SQL
        
        insert into HOSPITAL (nome, cod_hospital)
	    values
       	('Jayme', 10),
        ('Metropolitano', 17),
        ('Unimed Vitória', 18),
        ('Posto de Saúde', 12),
        ('Apart', 21),
        ('Santa Casa', 53),
        ('Santa Monica', 13),
        ('Vitoria Apart', 11),
        ('São camilo', 44);
        
        insert into PESSOA (nome, sexo, peso, altura, email, alergias, doencas_cronicas, tp_sanguineo, dt_nascimento, cpf, cep, n_carteirinha, n_sus, convenio, n_residencia, complemento, FK_BAIRRO_cod_bairro, )
	values
    ('Ricardo', 'M', 76, 180, 'ricardo@gmail.com', 'Pêlo de gato', 'Colesterol alto', 'AB+', '2001/03/10', '123.321.789-00', '21-189.122', '123.321.789', '123.321.700', 'Samp', 39, 'Casa', 55), 
    ('Maria', 'F', 45, 160, 'maria@gmail.com', 'Picada de mosquito', 'Nenhuma', 'AB-', '2002/03/03', '231.123.987-00', '20-190.091', '144.556.700', '144.556.789', 'São Bernardo', 880, 'Apartamento', 23),
    ('Lucas', 'M', 80, 190, 'lucas@gmail.com', 'Dermatite de contato', 'Nenhuma', 'AB-', '1999/12/10', '145.541.789-00', '19-123.098', '145.541.789', '876.678.123', 'Unimed', 34, 'Casa', 22), 
 	('Bernardo', 'M', 58, 177, 'bernardo@gmail.com', 'Nenhuma', 'Hipertensão', 'O-', '1998/09/12', '345.543.897-00', '18-234.097', '345.543.897', '789.876.321', 'Sus', 21, 'Casa alugada', 33), 
	('Leonardo', 'M', 78, 198, 'leonardo@gmail.com', 'Nenhuma', 'Diabete', 'AB+', '1999/01/04', '456.654.654-00', '17-345.096', '456.654.654', '123.321.789', 'Samp', 90, 'Apartamento', 45), 
	('Patricia', 'M', 34, 155, 'patricia@gmail.com', 'À poeira', 'Asma', 'AB+', '1997/09/08', '567.765.554-00', '16-456.095', '567.765.554', '144.556.700', 'Samp', 800, 'Apartamento', 21), 
	('Elisa', 'F', 50, 189, 'elisa@gmail.com', 'Rinite alérgica', 'Asma', 'AB-', '2001/11/16', '678.876.432-00', '15-567094', '678.876.432', '145.541.789', 'Samp', 765, 'Apartamento', 12), 
	('Carmem', 'F', 64, 179, 'carmem@gmail.com', 'Dermatite atópica', 'Nenhuma', 'O-', '1998/08/27', '789.876.321-00', '14-678093', '789.876.321', '345.543.897', 'Sus', 345, 'Casa', 39), 
	('Gustavo', 'M', 55, 198, 'gustavo@gmail.com', 'Nenhuma', 'Diabete', 'O-', '2001/07/12', '876.678.123-00', '13-789.092', '876.678.123', '456.654.654', 'Unimed', 654, 'Casa', 89);

    insert into DIAGNOSTICO (cod_diag, receita, doença) 
	values
    	(12, 'Dieta lvre de gordura', 'Colesterol'),
        (80, 'Analgésicos', 'Dengue'),
        (81, 'Insulina', 'Diabete'),
        (21, 'Vitamina', 'Anemina'),
        (22, 'Relaxamento', 'Enxaqueca'),
        (65, 'Antinflamatório', 'Resfriado'),
        (66, 'Anti-histaminico', 'Caxumba'),
        (43, 'Corticoide', 'Asma'),
        (47, 'Broncodilatador', 'Asma');
        
    INSERT INTO bairro (nome, cod_bairro, FK_CIDADE_cod_cidade) VALUES
    	('Laranjeiras', 54, 34),
	('Santa Rosa', 23, 33),
	('Itararé', 22, 33),	
	('Jacaraipe', 33, 34),
	('Itapuã', 45, 53 ),
	('jardim da Penha', 21, 33),
	('Vila Rubim', 12, 33),
	('Jacaraipe', 39, 34),
	('Itaparica', 89, 53);

  
    INSERT INTO cidade (nome, cod_cidade, FK_ESTADO_cod_estado) VALUES 
	      ('Serra', 34, 27),
	      ('Vitoria', 33, 27),
	      ('Pedra azul', 28, 27),
	      ('Cariacica', 44, 27),
      	('Vila Velha', 53, 27),
      	('Venda Nova', 35, 27),
	      ('Aracruz', 36, 27),
      	('Afonso Cláudio', 12, 27),
      	('Marechal Floriano', 66, 27);

    insert into trabalha (FK_PESSOA_CPF, FK_HOSPITAL_cod_hospital)
    	values
    		('456.654.654-00', 10),
        ('567.765.554-00', 17),
        ('678.876.432-00', 18),
        ('876.678.123-00', 12),
        ('567.765.554-00', 21),
        ('876.678.123-00', 53),
        ('876.678.123-00', 13),
        ('456.654.654-00', 11),
        ('567.765.554-00', 44); 
  
    INSERT INTO consulta (dt_consulta, hora, status, cod_consulta, FK_PESSOA_CPF, FK_HOSPITAL_cod_hospital, FK_DIAGNÓSTICO_cod_diag) VALUES 
	('2018/01/12', '18:00', 'Concluída', 21,'123.321.789-00',10, 12),
    ('2018/08/23', '12:00', 'Concluída',  8, '123.321.789-00', 17, 80),
    ('2018/08/23', '13:00', 'Concluída',  9, '231.123.987-00',18,81),
    ('2018/03/09', '9:00', 'Concluída',  12, '231.123.987-00',12, 21),
    ('2018/05/13', '14:00','Concluída', 14, '145.541.789-00',21, 22),
    ('2018/04/11', '8:00',	'Concluída', 56, '145.541.789-00',53, 65),
    ('2018/04/11', '9:30',	'Concluída', 57, '345.543.897-00',13, 66), 
    ('2018/04/11', '7:00', 'Concluída', 34, '345.543.897-00',11, 43),
    ('2018/07/12', '8:00',	'Concluída', 77, '456.654.654-00',44, 47);

#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script 
        (create para tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL
![Alter text]
(https://github.com/remedmax/trabalho01/blob/master/arquivos/create%2Binsercao.docx?raw=true "Dados")

#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
        a) Junção dos scripts anteriores em um único script 
        (Drop table + Create de tabelas e estruturas de dados + dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL

![Alter text]
(https://github.com/remedmax/trabalho01/blob/master/arquivos/drop%2Bcreate.docx?raw=true "Dados2")

![Alter text]
(https://github.com/remedmax/trabalho01/blob/master/imagens/8.3.png?raw=true "Drop")

### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
	
select * from pessoa;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/pessoa.png?raw=true "Pessoa")

select * from consulta;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/consulta.png?raw=true "Consulta")

select * from hospital;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/hospital.png?raw=true "Hospital")

select * from diagnóstico;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/diag.png?raw=true "Diagnostico")

select * from estado;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/estado.png?raw=true "Estado")

select * from cidade;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/cidade.png?raw=true "Cidade")

select * from bairro;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/bairro.png?raw=true "Bairro")

select * from hospital2;
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/createHosp2.png?raw=true "Hospital2")


#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

select * from diagnÓstico where doença = 'Asma';
select * from pessoa where sexo = 'F';
select * from consulta where hora >= '12:00';
select * from hospital where cod_hospital > 20;


#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not:
	select * from pessoa where tp_sanguineo = 'AB+' or sexo = 'M';
	select * from estado where cod_estado >= 11 and cod_estado <= 27;
	select * from consulta where cod_consulta > 12 and dt_consulta > '2018/01/12';
	select * from diagnostico where cod_diag >= 11 and cod_diag <= 27;
	select * from bairro where cod_bairro = 33 or cod_bairro = 45;

    b) Criar no mínimo 3 consultas com operadores aritméticos:
    	select * from pessoa where nome = 'Elisa';
	select * from diagnostico where receita = 'Insulina';
	select * from hospital where cod_hospital < 40;
    
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas:    	
	select sexo,tp_sanguineo as "tipo_sanguineo" from pessoa;
	alter table diagnÓstico rename to "diagnostico";
	select cod_estado as "codigo_estado" from estado;
	select dt_consulta,cod_consulta as "codigo_consulta" from consulta;

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.


    
#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>


#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        

## Marco de Entrega 02 em: (16/06/2018)<br>
### ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO SEMESTRAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (30/06/2018)
<br>

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

#### 9.11	LISTA DE CODIGOS DAS FUNÇÕES E TRIGGERS<br>
        Detalhamento sobre funcionalidade de cada código.
        a) Objetivo
        b) Código do objeto (função/trigger)
        c) exemplo de dados para aplicação
        d) resultados em forma de tabela/imagem
<br>


#### 9.12	GERACAO DE DADOS (MÍNIMO DE 100 MIL REGISTROS PARA PRINCIPAL RELAÇAO)<br>
        a) principal tabela do sistema deve ter no mínimo 100 mil registros
        b) tabelas diretamente relacionadas a tabela principal 10 mil registros
        c) tabelas auxiliares de relacao multivalorada mínimo de 10 registros
        d) registrar o tempo de inserção em cada uma das tabelas do banco de dados
        e) especificar a quantidade de registros inseridos em cada tabela
        Para melhor compreensão verifiquem o exemplo na base de testes:<br>
        https://github.com/discipbd2/base-de-testes-locadora
        

#### 9.13	Backup do Banco de Dados<br>
        Detalhamento do backup.
        a) Tempo
        b) Tamanho
        c) Teste de restauração (backup)
        d) Tempo para restauração
        e) Teste de restauração (script sql)
        f) Tempo para restauração (script sql)
<br>

Data de Entrega: (Data a ser definida)
<br>

#### 9.14	APLICAÇAO DE ÍNDICES E TESTES DE PERFORMANCE<br>
    a) Lista de índices, tipos de índices com explicação de porque foram implementados nas consultas 
    b) Performance esperada VS Resultados obtidos
    c) Tabela de resultados comparando velocidades antes e depois da aplicação dos índices (constando velocidade esperada com planejamento, sem indice e com índice Vs velocidade de execucao real com índice e sem índice).
    d) Escolher as consultas mais complexas para serem analisadas (consultas com menos de 2 joins não serão aceitas)
    e) As imagens do Explain devem ser inclusas no trabalho, bem como explicações sobre os resultados obtidos.
    f) Inclusão de tabela mostrando as 10 execuções, excluindo-se o maior e menor tempos para cada consulta e 
    obtendo-se a media dos outros valores como resultado médio final.
<br>
    Data de Entrega: (Data a ser definida)
<br>   

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 11 Backup completo do banco de dados postgres 
    a) deve ser realizado no formato "backup" 
        (Em Dump Options #1 Habilitar opções Don't Save Owner e Privilege)
    b) antes de postar o arquivo no git o mesmo deve ser testado/restaurado por outro grupo de alunos/dupla
    c) informar aqui o grupo de alunos/dupla que realizou o teste.

    
### 12	TUTORIAL COMPLETO DE PASSOS PARA RESTAURACAO DO BANCO E EXECUCAO DE PROCEDIMENTOS ENVOLVIDOS NO TRABALHO PARA OBTENÇÃO DOS RESULTADOS<br>
        a) Outros grupos deverão ser capazes de restaurar o banco 
        b) executar todas as consultas presentes no trabalho
        c) executar códigos que tenham sido construídos para o trabalho 
        d) realizar qualquer procedimento executado pelo grupo que desenvolveu o trabalho

### 13	DIFICULDADES ENCONTRADAS PELO GRUPO<br>  

    
>## Marco de Entrega 04/Entrega Final em: (Data definida no cronograma)<br>

       
### 14  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
   
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/

#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. Caso existam arquivos com conteúdos sigilosos, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário deste GIT, para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://sis4.com/brModelo/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


        
        


    





