# TRABALHO 01: REMEDMEX
Trabalho desenvolvido durante a disciplina de Banco de Dados do Integrado.

# Sumário

### 1.COMPONENTES<br>
Integrantes do grupo<br>
laira: lairaarruda@gmail.com<br>
maria eduarda: dudah.jbraga@gmail.com<br>
...

### 2.INTRODUÇÃO E MOTIVAÇAO<br>
Este documento contém a especificação do projeto do banco de dados <remedmax> 
<br>e motivação da escolha realizada. <br>
 
 > O sistema do aplicativo "remedmex" tem como intuito gerenciar a saúde das pessoas e auxiliar na organização profissional do médico, que seria o gestor. Para o usuário paciente, o intuito é que essa pessoa tenha registros sobre suas consultas, o que foi diagnosticado, qual a receita que o médico preescreveu e até mesmo informações sobre consultas que foram agendadas e não ocorreram ainda. já para o médico, o intuito é organizar o quadro de seus pacientes de forma particular e/ou generalizada, podendo analisar a ocorrência que uma doença possui em uma região. Se a ocôrrencia for frequente, os resultados apontam para uma possível epidemia. O objetivo é que o software ajude a diminuir os casos de pessoas que têm seus estados de saúde agravados por não terem buscado auxílio médico corretamente ou que não vão às suas consultas por terem se esquecido. Além disso, para o médico, torna-se essencial uma análise da conjuntura em que se encontram seus pacientes, que pode ser facilmente feita pelo remedmex. Nesse quesito, o aplicativo teria salvo em seus registros todos os detalhes sobre as consultas, diagnóosticos, médicos, hospitais, pacientes e formas de contato. Tudo para que o acesso às informações seja mais fácil e a relação entre paciente e médico seja mais próxima, que corrobora em uma rápida solução do problema do paciente.

### 3.MINI-MUNDO Novo<br>

Descrever o mini-mundo! (Não deve ser maior do que 30 linhas) <br>
Entrevista com o usuário e identificação dos requisitos.<br>
Descrição textual das regras de negócio definidas como um  subconjunto do mundo real 
cujos elementos são propriedades que desejamos incluir, processar, armazenar, 
gerenciar, atualizar, e que descrevem a proposta/solução a ser desenvolvida.

> O sistema proposto para o "remedmex" terá salvo em seu banco e dados as informações dos usuários para <b>cadastro</b>, que ficarão registradas em cada conta, assim como seu login e senha. Juntamente a essas informações, o usuário também irá informar outros dados, como por exemplo data de nascimento, sexo, peso, altura, email e, principalmente, o CPF. Contudo, também deverá informar dados de sua saúde, como: Convênio, número da carteirinha, número do sus, tipo sanguíneo, se faz uso de alguma medicação recorrente, se possui alguma doença crônica e/ou alguma alergia. Para ter controle sobre as regiões epidêmicas, solicita-se juntamente, informações sobre a localidade do usuário, tais como endereço, CEP, logradouro, bairro onde mora, cidade, estado, número da residência e complemento, caso houver. Se o usuário for um médico, deverá indicar sua especialidade também. 

O sistema armazenará em seu banco todas as informações pertibentes a uma consulta, como receita, data, horário, status, diagnóstico e doença, caso for constatada. A partir destas informações, o sistema gera uma série de tabelas e conjuntos de dados que servirão de base para consultas e análises sobre diversas perspectivas, como por exemplo, a relação entre a quantidade de médicos que existem de cada especialidade no hospital, ou a ocorrência de cada doença por região. As possibidades variam de acordo com a necessidade particular de cada um.

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser desenvolvidas. O princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas e/ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>


![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/baaaaaaay.png?raw=true "Modelo Conceitual")


![Arquivo PDF do Protótipo Balsamiq feito para Empresa Devcom]
(https://github.com/remedmax/trabalho01/blob/master/arquivos/remedmex.pdf?raw=true "Empresa Remedmex")


#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    a) O sistema proposto poderá fornecer quais tipos de relatórios e informaçes? 
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto!
    
> A remedemex precisa inicialmente dos seguintes relatórios:
* Relatório de cadastro que informe as seguintes informações sobre o paciente: nome e sobrenome, email, idade, sexo, peso e altura.
* Relatório de consulta que informará: hora e dia da consulta, código do status, código do diagnóstico, código do hospital, paciente e médico.
* Relatório de localidade que indicará: endereço completo do paciente ou médico, incluindo número da residência, complemento, logradouro, bairro, cidade e estado.
* Relatório com dados gerais para registrar a consulta que informará: o médico, hospital, data, diagnóstico e a receita.
* Relatório que armazenará uma diagnóstico, localizará o local e registrará: locais com epidemias.
 
 
#### 4.2 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
    
 ![Exemplo de Tabela de dados do Programa Remedmex](https://github.com/remedmax/trabalho01/blob/master/arquivos/DadosProgramaRemedmexAtt.xlsx?raw=true "Tabela - Programa Remedmex")
 
>## Marco de Entrega 01 em: (24/03/2018)<br>

### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
        * Para nosso prótótipo limitaremos o modelo conceitual nas 5 principais entidades do escopo
        * O protótipo deve possui no mínimo duas relações N para N
        * o mínimo de entidades do modelo conceitual será igual a 5
        
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/md_conceitualESSETACERTO.png?raw=true "Modelo Conceitual")



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
    [doenca - diagnostico]: decidimos não extender  a relação, para que o trabalho ficasse mais objetivo.

#### 5.3 DESCRIÇÃO DOS DADOS 
    [objeto]: [descrição do objeto]
    
    EXEMPLO:
    CLIENTE: Tabela que armazena as informações relativas ao cliente<br>
    CPF: campo que armazena o número de Cadastro de Pessoa Física para cada cliente da empresa.<br>
    
    Pessoa: Tabela que constitui os dados do usuario.
    CPF: Campo que armazena o número de Cadastro de Pessoa Física de cada usuario.
    CEP: Campo que determina a localização da pessoa.
    Email: Campo que informa um meio de comunicação.
    Sexo: Campo que determina o genero da pessoa.
    Altura: Campo que informa o tamanho da pessoa.
    Peso: Campo que informa quanto a pessoa pesa.
    Dt_nascimento: Campo que informa a idade da pessoa.
    Nº_carteirinha: Campo que informa o número de carteirinha da pessoa, caso ela tiver.
    Nº_sus: Campo que informa o número do sus, caso ela não tiver um convenio.
    Alergias: Campo que informa se a pessoa é ou não alérgica, caso for, mostra a alergia.
    Doenças_cronicas: Campo que informa se a pessoa contém ou não um tipo de doença cronica.
    Tp_sanguineo: Campo que informa o tipo sanguineo do usuario.
    Complemento: Campo que informa o tipo de lugar em que a pessoa mora, caso ela tiver.
    Convenio: Campo que informa o nome do convenio particular, caso a pessoa tiver.
    Nº_residencia: Campo que informa o numero do complemento.
    FK_bairro: Campo que informa o código de localização do bairro em que a pessoa mora.
    
    Hospital: Tabela que constitui os dados de cada hospital.
    Nome: Campo que indica o nome de um determinado hospital.
    Cod_hospital: Campo que atribui um codigo para o hospital.
    
    Estado: Tabela que constitui as informações de cada estado.
    Nome: Campo que indica o nome de um determinado estado.
    Cod_estado: Campo que atribui um codigo para o estado.
    
    Cidade: Tabela que constitui os dados de cada cidade.
    Nome: Campo que indica o nome de um determinado cidade.
    Cod_cidade: Campo que atribui um codigo para o cidade.
    FK_estado: Campo que informa o codigo do estado em que a cidade de localiza.
    
    Bairro: Tabela que constitui os dados de cada bairro.
    Nome: Campo que indica o nome de um determinado bairro.
    Cod_bairro: Campo que atribui um codigo para o bairro.
    FK_cidade: Campo que informa o codigo da cidade em que o bairro de localiza.
    
    Diagnóstico: Tabela que constitui as informações após a consulta.
    Cod_diag: Campo que atribui um codigo para identificar uma receita e doença.
    Receita: Campo  que informa o tratamento.
    Doença: Campo que informa o que o usuario tem.
    
    Consulta: Tabela que constitui todas as informações do atendimento ao usuario.
    Dt_consulta: Campo que indica a data em que o usuario foi atendido.
    Horas: Campo que informa o horário da consulta.
    Status: Campo que indica se a consulta foi, ou não realizada.
    Fk_pessoa_cpf: Campo que indicada o cpf da pessoa consultada.
    Fk_hospital: Campo que indica o hospital em que o atendimento foi feito.
    Fk_bairro: Campo que indica o bairro em que a pessoa e o hospital se localiza.


>## Marco de Entrega 01 em: (12/05/2018)<br>
### 6	MODELO LÓGICO<br>
        a) inclusão do modelo lógico do banco de dados:
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/L%C3%B3gico_1.png?raw=true "Modelo Lógico")
   
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)

### 7	MODELO FÍSICO<br>
        a) inclusão das instruções de criacão das estruturas DDL 
        (criação de tabelas, alterações, etc..)         
    /* Lógico_1: */

	CREATE TABLE PESSOA (
	    email varchar(45),
	    altura int,
	    CPF varchar(45) PRIMARY KEY,
	    dt_nascimento date,
	    peso double,
	    nome varchar(30),
	    FK_TP_SANGUINEO_cod_tp_sanguineo int,
	    FK_SEXO_cod_sexo int
	);

	CREATE TABLE CONSULTA (
	    data date,
	    hora datetime,
	    cod_consulta int PRIMARY KEY,
	    FK_MÉDICO_FK_PESSOA_CPF varchar(45),
	    FK_HOSPITAL_cod_hospital int,
	    FK_DIAGNOSTICO_cod_diag int,
	    FK_PESSOA_CPF varchar(45),
	    hora_agenda datetime,
	    data_agenda date,
	    FK_STATUS_cod_status int
	);

	CREATE TABLE HOSPITAL (
	    nome_hospital varchar(30),
	    cod_hospital int PRIMARY KEY,
	    FK_ENDERECO_cod_endereco int
	);

	CREATE TABLE MÉDICO (
	    FK_PESSOA_CPF varchar(45) PRIMARY KEY
	);

	CREATE TABLE DIAGNOSTICO (
	    cod_diag int PRIMARY KEY,
	    receita varchar(30)
	);

	CREATE TABLE BAIRRO (
	    nome_bairro varchar(30),
	    cod_bairro int PRIMARY KEY,
	    FK_CIDADE_cod_cidade int
	);

	CREATE TABLE CIDADE (
	    nome_cidade varchar(30),
	    cod_cidade int PRIMARY KEY,
	    FK_ESTADO_cod_estado int
	);

	CREATE TABLE ESTADO (
	    nome_estado varchar(30),
	    cod_estado int PRIMARY KEY
	);

	CREATE TABLE DOENÇA (
	    cod_doenca int PRIMARY KEY,
	    nome_doenca string
	);
	
	CREATE TABLE ALERGIA (
	    nome_alergia varchar(20),
	    cod_alergia int PRIMARY KEY
	);

	CREATE TABLE DOENCA_CRONICA (
	    nome_doenca_c varchar(30),
	    cod_doenca_c int PRIMARY KEY
	);

	CREATE TABLE TP_SANGUINEO (
	    nome_tp_sanguineo varchar(20),
	    cod_tp_sanguineo int PRIMARY KEY
	);
	
	CREATE TABLE PLANO_SAUDE (
	    num_carteirinha int PRIMARY KEY
	);

	CREATE TABLE ESPECIALIDADE_MED (
	    nome_especialidade varchar(30),
	    cod_especialidade int PRIMARY KEY
	);

	CREATE TABLE ENDERECO (
	    CEP varchar(20),
	    num_imovel int,
	    cod_endereco int PRIMARY KEY,
	    FK_BAIRRO_cod_bairro int
	);

	CREATE TABLE COMPLEMENTO (
	    complemento varchar(45),
	    cod_comp int PRIMARY KEY,
	    FK_ENDERECO_cod_endereco int
	);

	CREATE TABLE CONTATO (
	    cod int PRIMARY KEY,
	    desc varchar(20),
	    FK_TIPO_CONTATO_cod int
	);

	CREATE TABLE TIPO_CONTATO (
	    cod int PRIMARY KEY,
	    desc_tipo varchar(20)
	);

	CREATE TABLE CONVENIO (
	    nome varchar(20),
	    FK_PLANO_SAUDE_num_carteirinha int PRIMARY KEY
	);

	CREATE TABLE SEXO (
	    tipo_sexo varchar(20),
	    cod_sexo int PRIMARY KEY
	);

	CREATE TABLE LOGRADOURO (
	    cod_logra int PRIMARY KEY,
	    tp_logra varchar(20)
	);

	CREATE TABLE STATUS (
	    cod_status int PRIMARY KEY,
	    tp_status varchar(20)
	);

	CREATE TABLE Trabalha (
	    fk_HOSPITAL_cod_hospital int,
	    fk_MÉDICO_FK_PESSOA_CPF varchar(45)
	);

	CREATE TABLE Diag_Doenca (
	    fk_DIAGNOSTICO_cod_diag int,
	    fk_DOENÇA_cod_doenca int
	);

	CREATE TABLE Pessoa_A (
	    fk_ALERGIA_cod_alergia int,
	    fk_PESSOA_CPF varchar(45)
	);

	CREATE TABLE Pessoa_DC (
	    fk_DOENCA_CRONICA_cod_doenca_c int,
	    fk_PESSOA_CPF varchar(45)
	);

	CREATE TABLE Pesoa_PS (
	    fk_PLANO_SAUDE_num_carteirinha int,
	    fk_PESSOA_CPF varchar(45)
	);

	CREATE TABLE Med_Esp (
	    fk_MÉDICO_FK_PESSOA_CPF varchar(45),
	    fk_ESPECIALIDADE_MED_cod_especialidade int
	);

	CREATE TABLE Pessoa_End (
	    fk_PESSOA_CPF varchar(45),
	    fk_ENDERECO_cod_endereco int
	);

	CREATE TABLE Contato_Pessoa (
	    fk_PESSOA_CPF varchar(45),
	    fk_CONTATO_cod int
	);

	CREATE TABLE End_Logra (
	    fk_LOGRADOURO_cod_logra int,
	    fk_ENDERECO_cod_endereco int
	);
 
	ALTER TABLE PESSOA ADD CONSTRAINT FK_PESSOA_2
	    FOREIGN KEY (FK_TP_SANGUINEO_cod_tp_sanguineo)
	    REFERENCES TP_SANGUINEO (cod_tp_sanguineo)
	    ON DELETE CASCADE;
 
	ALTER TABLE PESSOA ADD CONSTRAINT FK_PESSOA_3
	    FOREIGN KEY (FK_SEXO_cod_sexo)
	    REFERENCES SEXO (cod_sexo)
	    ON DELETE CASCADE;
 
	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_2
	    FOREIGN KEY (FK_MÉDICO_FK_PESSOA_CPF)
	    REFERENCES MÉDICO (FK_PESSOA_CPF)
	    ON DELETE CASCADE;
 
	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_3
	    FOREIGN KEY (FK_HOSPITAL_cod_hospital)
	    REFERENCES HOSPITAL (cod_hospital)
	    ON DELETE CASCADE;

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_4
	    FOREIGN KEY (FK_DIAGNOSTICO_cod_diag)
	    REFERENCES DIAGNOSTICO (cod_diag)
	    ON DELETE RESTRICT;

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_5
	    FOREIGN KEY (FK_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE CASCADE;
 
	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_6
	    FOREIGN KEY (FK_STATUS_cod_status)
	    REFERENCES STATUS (cod_status)
	    ON DELETE CASCADE;

	ALTER TABLE HOSPITAL ADD CONSTRAINT FK_HOSPITAL_2
	    FOREIGN KEY (FK_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE CASCADE;

	ALTER TABLE MÉDICO ADD CONSTRAINT FK_MÉDICO_2
	    FOREIGN KEY (FK_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE CASCADE;

	ALTER TABLE BAIRRO ADD CONSTRAINT FK_BAIRRO_2
	    FOREIGN KEY (FK_CIDADE_cod_cidade)
	    REFERENCES CIDADE (cod_cidade)
	    ON DELETE RESTRICT;

	ALTER TABLE CIDADE ADD CONSTRAINT FK_CIDADE_2
	    FOREIGN KEY (FK_ESTADO_cod_estado)
	    REFERENCES ESTADO (cod_estado)
	    ON DELETE RESTRICT;

	ALTER TABLE ENDERECO ADD CONSTRAINT FK_ENDERECO_2
	    FOREIGN KEY (FK_BAIRRO_cod_bairro)
	    REFERENCES BAIRRO (cod_bairro)
	    ON DELETE RESTRICT;

	ALTER TABLE COMPLEMENTO ADD CONSTRAINT FK_COMPLEMENTO_2
	    FOREIGN KEY (FK_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE CASCADE;
 
	ALTER TABLE CONTATO ADD CONSTRAINT FK_CONTATO_2
	    FOREIGN KEY (FK_TIPO_CONTATO_cod)
	    REFERENCES TIPO_CONTATO (cod)
	    ON DELETE RESTRICT;

	ALTER TABLE CONVENIO ADD CONSTRAINT FK_CONVENIO_2
	    FOREIGN KEY (FK_PLANO_SAUDE_num_carteirinha)
	    REFERENCES PLANO_SAUDE (num_carteirinha)
	    ON DELETE CASCADE;

	ALTER TABLE Trabalha ADD CONSTRAINT FK_Trabalha_1
	    FOREIGN KEY (fk_HOSPITAL_cod_hospital)
	    REFERENCES HOSPITAL (cod_hospital)
	    ON DELETE RESTRICT;

	ALTER TABLE Trabalha ADD CONSTRAINT FK_Trabalha_2
	    FOREIGN KEY (fk_MÉDICO_FK_PESSOA_CPF)
	    REFERENCES MÉDICO (FK_PESSOA_CPF)
	    ON DELETE SET NULL;

	ALTER TABLE Diag_Doenca ADD CONSTRAINT FK_Diag_Doenca_1
	    FOREIGN KEY (fk_DIAGNOSTICO_cod_diag)
	    REFERENCES DIAGNOSTICO (cod_diag)
	    ON DELETE RESTRICT;

	ALTER TABLE Diag_Doenca ADD CONSTRAINT FK_Diag_Doenca_2
	    FOREIGN KEY (fk_DOENÇA_cod_doenca)
	    REFERENCES DOENÇA (cod_doenca)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_A ADD CONSTRAINT FK_Pessoa_A_1
	    FOREIGN KEY (fk_ALERGIA_cod_alergia)
	    REFERENCES ALERGIA (cod_alergia)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_A ADD CONSTRAINT FK_Pessoa_A_2
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_DC ADD CONSTRAINT FK_Pessoa_DC_1
	    FOREIGN KEY (fk_DOENCA_CRONICA_cod_doenca_c)
	    REFERENCES DOENCA_CRONICA (cod_doenca_c)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_DC ADD CONSTRAINT FK_Pessoa_DC_2
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE SET NULL;

	ALTER TABLE Pesoa_PS ADD CONSTRAINT FK_Pesoa_PS_1
	    FOREIGN KEY (fk_PLANO_SAUDE_num_carteirinha)
	    REFERENCES PLANO_SAUDE (num_carteirinha)
	    ON DELETE RESTRICT;

	ALTER TABLE Pesoa_PS ADD CONSTRAINT FK_Pesoa_PS_2
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE SET NULL;

	ALTER TABLE Med_Esp ADD CONSTRAINT FK_Med_Esp_1
	    FOREIGN KEY (fk_MÉDICO_FK_PESSOA_CPF)
	    REFERENCES MÉDICO (FK_PESSOA_CPF)
	    ON DELETE RESTRICT;

	ALTER TABLE Med_Esp ADD CONSTRAINT FK_Med_Esp_2
	    FOREIGN KEY (fk_ESPECIALIDADE_MED_cod_especialidade)
	    REFERENCES ESPECIALIDADE_MED (cod_especialidade)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_End ADD CONSTRAINT FK_Pessoa_End_1
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE RESTRICT;

	ALTER TABLE Pessoa_End ADD CONSTRAINT FK_Pessoa_End_2
	    FOREIGN KEY (fk_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE RESTRICT;

	ALTER TABLE Contato_Pessoa ADD CONSTRAINT FK_Contato_Pessoa_1
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE RESTRICT;

	ALTER TABLE Contato_Pessoa ADD CONSTRAINT FK_Contato_Pessoa_2
	    FOREIGN KEY (fk_CONTATO_cod)
	    REFERENCES CONTATO (cod)
	    ON DELETE SET NULL;

	ALTER TABLE End_Logra ADD CONSTRAINT FK_End_Logra_1
	    FOREIGN KEY (fk_LOGRADOURO_cod_logra)
	    REFERENCES LOGRADOURO (cod_logra)
	    ON DELETE SET NULL;

	ALTER TABLE End_Logra ADD CONSTRAINT FK_End_Logra_2
	    FOREIGN KEY (fk_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE SET NULL;
         
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físic
        b) formato .SQL

	CREATE TABLE ESTADO (
	    nome_estado varchar(30),
	    cod_estado int PRIMARY KEY
	);
	INSERT INTO estado (nome_estado, cod_estado) VALUES 
		('Espírito Santo', 27),
		('São Paulo', 11),
		('Bahia', 71),
		('Rio de Janeiro', 21),
		('Minas Gerais', 33),
		('Paraná', 41),
		('Goiás', 62),
		('Amazonas', 92),
		('Santa Catarina', 47);

	CREATE TABLE CIDADE (
	    nome_cidade varchar(30),
	    cod_cidade int PRIMARY KEY,
	    FK_ESTADO_cod_estado int
	);
	
	ALTER TABLE CIDADE ADD CONSTRAINT FK_CIDADE_2
	    FOREIGN KEY (FK_ESTADO_cod_estado)
	    REFERENCES ESTADO (cod_estado)
	    ON DELETE RESTRICT;
	    
	INSERT INTO cidade (nome_cidade, cod_cidade, FK_ESTADO_cod_estado) VALUES 
		('Serra', 34, 27),
		('Vitória', 33, 27),
		('Pedra azul', 28, 27),
		('Cariacica', 44, 27),
		('Vila Velha', 53, 27),
		('Venda Nova', 35, 27),
		('Aracruz', 36, 27),
		('Afonso Cláudio', 12, 27),
		('Marechal Floriano', 66, 27);



	CREATE TABLE BAIRRO (
	    nome_bairro varchar(30),
	    cod_bairro int PRIMARY KEY,
	    FK_CIDADE_cod_cidade int
	);
	
	ALTER TABLE BAIRRO ADD CONSTRAINT FK_BAIRRO_2
	    FOREIGN KEY (FK_CIDADE_cod_cidade)
	    REFERENCES CIDADE (cod_cidade)
	    ON DELETE RESTRICT;
	    
	INSERT INTO bairro (nome_bairro, cod_bairro, FK_CIDADE_cod_cidade) VALUES
	('Laranjeiras', 10, 34),
	('Santa Rosa', 1, 33),
	('Itararé', 2, 33),	
	('Jacaraipe', 3, 34),
	('Itapuã', 4, 53 ),
	('jardim da Penha', 5, 33),
	('Vila Rubim', 6, 33),
	('Jacaraipe', 7, 34),
	('Itaparica', 8, 53);

	CREATE TABLE ENDERECO (
	    CEP varchar(20),
	    num_imovel int,
	    cod_endereco int PRIMARY KEY,
	    FK_BAIRRO_cod_bairro int
	);

	ALTER TABLE ENDERECO ADD CONSTRAINT FK_ENDERECO_2
	    FOREIGN KEY (FK_BAIRRO_cod_bairro)
	    REFERENCES BAIRRO (cod_bairro)
	    ON DELETE RESTRICT;
	    
	insert into endereco(CEP, cod_endereco, num_imovel, FK_BAIRRO_cod_bairro  ) values
	('12345-123',11,9,1),
	('23456-123',22,8,1),
	('34567-321',33,7,2),
	('45678-231',44,6,3),
	('56789-132',55,5,4),
	('67890-123',66,4,5),
	('78901-321',77,3,6),
	('89012-213',88,2,7),
	('99012-223',99,1,8);

	CREATE TABLE LOGRADOURO (
	    cod_logra int PRIMARY KEY,
	    tp_logra varchar(20)
	);
	
	insert into LOGRADOURO (cod_logra, tp_logra) values
	(1, 'bairro'),
	(2, 'estrada'),
	(3, 'avenida'),
	(4, 'rua'),
	(5, 'rodovia'),
	(6, 'trevo'),
	(7, 'vila'),
	(8, 'residencial'),
	(9, 'fazenda'),
	(10, 'distrito'),
	(11, 'viaduto');

	CREATE TABLE End_Logra (
	    fk_LOGRADOURO_cod_logra int,
	    fk_ENDERECO_cod_endereco int
	);
	ALTER TABLE End_Logra ADD CONSTRAINT FK_End_Logra_1
	    FOREIGN KEY (fk_LOGRADOURO_cod_logra)
	    REFERENCES LOGRADOURO (cod_logra)
	    ON DELETE SET NULL;

	ALTER TABLE End_Logra ADD CONSTRAINT FK_End_Logra_2
	    FOREIGN KEY (fk_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE SET NULL;
	    
	insert into End_Logra(fk_LOGRADOURO_cod_logra , fk_ENDERECO_cod_endereco )values
	(9, 11), 
	(8, 22), 
	(7, 33), 
	(6, 44), 
	(11, 55), 
	(5, 66), 
	(1, 77);

	CREATE TABLE COMPLEMENTO (
	    complemento varchar(45),
	    cod_comp int PRIMARY KEY,
	    FK_ENDERECO_cod_endereco int
	);
	
	ALTER TABLE COMPLEMENTO ADD CONSTRAINT FK_COMPLEMENTO_2
	    FOREIGN KEY (FK_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE CASCADE;
	    
	insert into COMPLEMENTO (complemento, cod_comp, fk_ENDERECO_cod_endereco) values
	('D-1203',1,77), 
	('F-405',2,66), 
	('A-123',3,55), 
	('N-309',4,44), 
	('C-403',5,33), 
	('E-208',6,22), 
	('D-1004',7,11);
	
	CREATE TABLE SEXO (
	    tipo_sexo varchar(20),
	    cod_sexo int PRIMARY KEY
	);
	
	insert into SEXO(tipo_sexo, cod_sexo)values
	('feminino', 1), 
	( 'Masculino', 2), 
	( 'outro', 3);

	CREATE TABLE TIPO_CONTATO (
	    cod int PRIMARY KEY,
	    desc_tipo varchar(20)
	);
	
	insert into TIPO_CONTATO(cod, desc_tipo) values
	(1, 'celular'),
	(2, 'fixo'),
	(3, 'twitter'),
	(4, 'facebook'),
	(5, 'comercial'),
	(6, 'msn'),
	(7, 'orkut');
	
	CREATE TABLE CONTATO (
	    cod int PRIMARY KEY,
	    descricao varchar(20),
	    FK_TIPO_CONTATO_cod int
	);
	
	ALTER TABLE CONTATO ADD CONSTRAINT FK_CONTATO_2
	    FOREIGN KEY (FK_TIPO_CONTATO_cod)
	    REFERENCES TIPO_CONTATO (cod)
	    ON DELETE RESTRICT;
	    
	insert into CONTATO(FK_TIPO_CONTATO_cod, descricao, cod) values 
	(1, '9998869593', 7),
	(2, '32816891', 6),
	(3, '@mkr123', 5),
	(4, '@RicardoRamos', 4),
	(6, '@elisalindinha', 3),
	(7, '@bonitaodobairro', 2);
	
	CREATE TABLE PLANO_SAUDE (
	    num_carteirinha int PRIMARY KEY
	);
	insert into plano_saude(num_carteirinha )values 
	(123456), 
	(234567), 
	(3456789), 
	(4567890), 
	(5678901);

	CREATE TABLE CONVENIO (
	    nome varchar(20),
	    FK_PLANO_SAUDE_num_carteirinha int PRIMARY KEY
	);

	ALTER TABLE CONVENIO ADD CONSTRAINT FK_CONVENIO_2
	    FOREIGN KEY (FK_PLANO_SAUDE_num_carteirinha)
	    REFERENCES PLANO_SAUDE (num_carteirinha)
	    ON DELETE CASCADE;
	    
	insert into convenio(nome , FK_PLANO_SAUDE_num_carteirinha  ) values 
	('São Bernardo', 123456), 
	('Samp', 234567 ), 
	('Unimed', 3456789), 
	('Med senior', 4567890), 
	('SUS', 5678901);

	CREATE TABLE TP_SANGUINEO (
	    nome_tp_sanguineo varchar(20),
	    cod_tp_sanguineo int PRIMARY KEY
	);
	
	insert into tp_sanguineo(nome_tp_sanguineo , cod_tp_sanguineo ) values
	('AB+', 1), 
	( 'AB-', 2), 
	( 'O+', 3),
	 ( 'O-', 4), 
	( 'A+', 5), 
	( 'A-', 6);
	
	CREATE TABLE DOENCA_CRONICA (
	    nome_doenca_c varchar(30),
	    cod_doenca_c int PRIMARY KEY
	);

	insert into DOENCA_CRONICA (nome_doenca_c, cod_doenca_c) values
	('Hipertensão arterial', 1),
	('Diabetes', 2),
	('Aids', 3),
	('Câncer', 4),
	('Asma', 5),
	('Colesterol alto', 6);

	CREATE TABLE ALERGIA (
	    nome_alergia varchar(20),
	    cod_alergia int PRIMARY KEY
	);
	
	insert into ALERGIA (nome_alergia, cod_alergia) values
	('poeira', 1),
	('pelo de gato', 2),
	('frutos do mar', 3),
	('lactose', 4),
	('nenhuma', 5);
	
	CREATE TABLE Pessoa_End (
	    fk_PESSOA_CPF varchar(45),
	    fk_ENDERECO_cod_endereco int
	);
	
	ALTER TABLE Pessoa_End ADD CONSTRAINT FK_Pessoa_End_1
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE RESTRICT;

	ALTER TABLE Pessoa_End ADD CONSTRAINT FK_Pessoa_End_2
	    FOREIGN KEY (fk_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE RESTRICT;
	    
	insert into Pessoa_End(fk_PESSOA_CPF , fk_ENDERECO_cod_endereco ) values ('123.321.789-00', 11), 
	('231.321.987-00', 22), 
	('145.541.789-00', 33), 
	('345.543.897-00', 44), 
	('456.654.654-00', 55), 
	('567.765.554-00', 66);
	
	CREATE TABLE Contato_Pessoa (
	    fk_PESSOA_CPF varchar(45),
	    fk_CONTATO_cod int
	);
	
	ALTER TABLE Contato_Pessoa ADD CONSTRAINT FK_Contato_Pessoa_1
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE RESTRICT;

	ALTER TABLE Contato_Pessoa ADD CONSTRAINT FK_Contato_Pessoa_2
	    FOREIGN KEY (fk_CONTATO_cod)
	    REFERENCES CONTATO (cod)
	    ON DELETE SET NULL;
	    
	insert into Contato_Pessoa (fk_PESSOA_CPF, fk_CONTATO_cod) values
	('123.321.789-00', 7),
	('231.321.987-00', 6),
	('567.765.554-00', 5),
	('123.321.789-00', 4),
	('678.876.432-00', 3),
	('456.654.654-00', 2);

	CREATE TABLE Pessoa_A (
	    fk_ALERGIA_cod_alergia int,
	    fk_PESSOA_CPF varchar(45)
	);

	ALTER TABLE Pessoa_A ADD CONSTRAINT FK_Pessoa_A_1
	    FOREIGN KEY (fk_ALERGIA_cod_alergia)
	    REFERENCES ALERGIA (cod_alergia)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_A ADD CONSTRAINT FK_Pessoa_A_2
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE SET NULL;
	    
	insert into PESSOA_A (fk_ALERGIA_cod_alergia, fk_PESSOA_CPF) values
	(1, '123.321.789-00'),
	(2, '231.321.987-00'),
	(3, '567.765.554-00'),
	(4, '123.321.789-00'),
	(5, '456.654.654-00');


	CREATE TABLE Pessoa_PS (
	    fk_PLANO_SAUDE_num_carteirinha int,
	    fk_PESSOA_CPF varchar(45)
	);
	
	ALTER TABLE Pessoa_PS ADD CONSTRAINT FK_Pesoa_PS_1
	    FOREIGN KEY (fk_PLANO_SAUDE_num_carteirinha)
	    REFERENCES PLANO_SAUDE (num_carteirinha)
	    ON DELETE RESTRICT;

	ALTER TABLE Pessoa_PS ADD CONSTRAINT FK_Pesoa_PS_2
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE SET NULL;
	    
	insert into Pessoa_PS (fk_PLANO_SAUDE_num_carteirinha, fk_PESSOA_CPF) values
	(123456, '123.321.789-00'),
	(234567,'231.321.987-00'),
	(3456789,'567.765.554-00'),
	(4567890,'123.321.789-00'),
	(5678901,'456.654.654-00');
	
	CREATE TABLE Pessoa_DC (
	    fk_DOENCA_CRONICA_cod_doenca_c int,
	    fk_PESSOA_CPF varchar(45));

	ALTER TABLE Pessoa_DC ADD CONSTRAINT FK_Pessoa_DC_1
	    FOREIGN KEY (fk_DOENCA_CRONICA_cod_doenca_c)
	    REFERENCES DOENCA_CRONICA (cod_doenca_c)
	    ON DELETE SET NULL;

	ALTER TABLE Pessoa_DC ADD CONSTRAINT FK_Pessoa_DC_2
	    FOREIGN KEY (fk_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE SET NULL;

	insert into Pessoa_DC (fk_DOENCA_CRONICA_cod_doenca_c, fk_PESSOA_cpf) values
	(1, '123.321.789-00'),
	(2, '231.321.987-00'),
	(3, '145.541.789-00'),
	(4, '345.543.897-00'),
	(5, '456.654.654-00'),
	(6, '876.678.123-00');
	
	CREATE TABLE PESSOA (
	    email varchar(45),
	    altura int,
	    CPF varchar(45) PRIMARY KEY,
	    dt_nascimento date,
	    peso int,
	    nome varchar(30),
	    FK_TP_SANGUINEO_cod_tp_sanguineo int,
	    FK_SEXO_cod_sexo int
	);
	
	ALTER TABLE PESSOA ADD CONSTRAINT FK_PESSOA_2
	    FOREIGN KEY (FK_TP_SANGUINEO_cod_tp_sanguineo)
	    REFERENCES TP_SANGUINEO (cod_tp_sanguineo)
	    ON DELETE CASCADE;

	ALTER TABLE PESSOA ADD CONSTRAINT FK_PESSOA_3
	    FOREIGN KEY (FK_SEXO_cod_sexo)
	    REFERENCES SEXO (cod_sexo)
	    ON DELETE CASCADE;

	insert into PESSOA (nome, FK_SEXO_cod_sexo, peso, altura, email, FK_TP_SANGUINEO_cod_tp_sanguineo, dt_nascimento, cpf)
	values
	('Ricardo', 2, 76, 180, 'ricardo@gmail.com', 1, '2001/03/10', '123.321.789-00'), 
	('Maria', 1, 45, 160, 'maria@gmail.com',2, '2002/03/03', '231.321.987-00'),
	('Lucas', 2, 80, 190, 'lucas@gmail.com',3, '1999/12/10', '145.541.789-00'), 
	('Bernardo', 3, 58, 177, 'bernardo@gmail.com',4, '1998/09/12', '345.543.897-00'), 
	('Leonardo', 3, 78, 198, 'leonardo@gmail.com', 5, '1999/01/04', '456.654.654-00'), 
	('Patricia', 1, 34, 155, 'patricia@gmail.com',4, '1997/09/08', '567.765.554-00'), 
	('Elisa', 1, 50, 189, 'elisa@gmail.com',5, '2001/11/16', '678.876.432-00'), 
	('Carmem', 1, 64, 179, 'carmem@gmail.com', 6, '1998/08/27', '789.876.321-00'), 
	('Gustavo', 2, 55, 198, 'gustavo@gmail.com', 5, '2001/07/12', '876.678.123-00');
	
	CREATE TABLE MEDICO (
	    FK_PESSOA_CPF varchar(45) PRIMARY KEY
	);
	
	ALTER TABLE MEDICO ADD CONSTRAINT FK_MÉDICO_2
	    FOREIGN KEY (FK_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE CASCADE;

	insert into medico (FK_PESSOA_CPF) values
		('345.543.897-00'),
		('123.321.789-00'),
		('231.321.987-00'),
		('145.541.789-00'),
	('567.765.554-00');
	
	CREATE TABLE ESPECIALIDADE_MED (
	    nome_especialidade varchar(30),
	    cod_especialidade int PRIMARY KEY);

	INSERT INTO especialidade_med (nome_especialidade, cod_especialidade) VALUES
	('Cardiologista', 1),
	('Infectologista',2),
	('Endocrinologista',3),
	('Cardiologista',4),
	('Clínico Geral',6);
	MÉDICO_ESPECIALIDADE
	CREATE TABLE Med_Esp (
	    fk_MÉDICO_FK_PESSOA_CPF varchar(45),
	    fk_ESPECIALIDADE_MED_cod_especialidade int
	);

	ALTER TABLE Med_Esp ADD CONSTRAINT FK_Med_Esp_1
	    FOREIGN KEY (fk_MÉDICO_FK_PESSOA_CPF)
	    REFERENCES MEDICO (FK_PESSOA_CPF)
	    ON DELETE RESTRICT;

	ALTER TABLE Med_Esp ADD CONSTRAINT FK_Med_Esp_2
	    FOREIGN KEY (fk_ESPECIALIDADE_MED_cod_especialidade)
	    REFERENCES ESPECIALIDADE_MED (cod_especialidade)
	    ON DELETE SET NULL;
	    
	insert into Med_esp (fk_ESPECIALIDADE_MED_cod_especialidade, fk_MÉDICO_FK_PESSOA_CPF ) values
	(1, '345.543.897-00'),
	(2, '123.321.789-00'),
	(3, '231.321.987-00'),
	(4, '145.541.789-00'),
	(6, '567.765.554-00');
	
	CREATE TABLE DOENCA (
	    cod_doenca int PRIMARY KEY,
	    nome_doenca varchar(40)
	);

	insert into DOENCA (cod_doenca, nome_doenca) 
	values
	    (13, 'Colesterol'),
	    (81, 'Dengue'),
	    (82, 'Diabete'),
	    (23, 'Anemina'),
	    (24, 'Enxaqueca'),
	    (66, 'Resfriado'),
	    (67, 'Caxumba'),
	    (44, 'Asma'),
	    (22, 'hepatite'),
	 (48, 'bronquite');

	CREATE TABLE DIAGNOSTICO (
	    cod_diag int PRIMARY KEY,
	    receita varchar(30)
	);
	
	insert into DIAGNOSTICO (cod_diag, receita) 
	values
	    (12, 'Dieta livre de gordura'),
	    (80, 'Analgésicos'),
	    (81, 'Insulina'),
	    (21, 'Vitamina'),
	    (22, 'Relaxamento'),
	    (65, 'Antinflamatório'),
	    (66, 'Anti-histaminico'),
	    (43, 'Corticoide'),
	    (47, 'Broncodilatador');
	
	CREATE TABLE Diag_Doenca (
	    fk_DIAGNOSTICO_cod_diag int,
	    fk_DOENÇA_cod_doenca int
	);
	
	ALTER TABLE Diag_Doenca ADD CONSTRAINT FK_Diag_Doenca_1
	    FOREIGN KEY (fk_DIAGNOSTICO_cod_diag)
	    REFERENCES DIAGNOSTICO (cod_diag)
	    ON DELETE RESTRICT;

	ALTER TABLE Diag_Doenca ADD CONSTRAINT FK_Diag_Doenca_2
	    FOREIGN KEY (fk_DOENÇA_cod_doenca)
	    REFERENCES DOENCA (cod_doenca)
	    ON DELETE SET NULL;
	    
	insert into diag_doenca(fk_DIAGNOSTICO_cod_diag , fk_DOENÇA_cod_doenca )values 
	(12, 13), (80, 81), (81, 82), (21, 23), (22, 22), (65, 66), (66, 67), (43, 44), (47, 48);

	CREATE TABLE STATUS (
	    cod_status int PRIMARY KEY,
	    tp_status varchar(20)
	);
	
	insert into status (cod_status , tp_status )values(1, 'Concluída'), (2, 'não concluída');
	
	CREATE TABLE HOSPITAL (
	    nome_hospital varchar(30),
	    cod_hospital int PRIMARY KEY,
	    FK_ENDERECO_cod_endereco int
	);

	ALTER TABLE HOSPITAL ADD CONSTRAINT FK_HOSPITAL_2
	    FOREIGN KEY (FK_ENDERECO_cod_endereco)
	    REFERENCES ENDERECO (cod_endereco)
	    ON DELETE CASCADE;
	    
	insert into HOSPITAL (nome_hospital, cod_hospital, FK_ENDERECO_cod_endereco )
	    values
	   ('Jayme', 10, 11),
	    ('Metropolitano', 17, 22),
	    ('Unimed Vitória', 18, 33),
	    ('Posto de Saúde', 12, 44),
	    ('Apart', 21, 44),
	    ('Santa Casa', 53, 55),
	    ('Santa Monica', 13, 55),
	    ('Vitoria Apart', 9, 66),
	    ('São camilo', 44, 77);
	
	CREATE TABLE Trabalha (
	    fk_HOSPITAL_cod_hospital int,
	    fk_MÉDICO_FK_PESSOA_CPF varchar(45)
	);

	ALTER TABLE Trabalha ADD CONSTRAINT FK_Trabalha_2
	    FOREIGN KEY (fk_MÉDICO_FK_PESSOA_CPF)
	    REFERENCES MEDICO (FK_PESSOA_CPF)
	    ON DELETE SET NULL;
	    
	insert into trabalha(fk_HOSPITAL_cod_hospital , fk_MÉDICO_FK_PESSOA_CPF ) values
	(10, '345.543.897-00' ), 
	(17, '123.321.789-00'),
	(18, '231.321.987-00'), 
	(12, '145.541.789-00'), 
	(21, '145.541.789-00'), 
	(53, '567.765.554-00'), 
	(13, '567.765.554-00'), 
	(9, '345.543.897-00'), 
	(44, '345.543.897-00');
	
	CREATE TABLE CONSULTA (
	    dt_consulta date,
	    hora time,
	    cod_consulta int PRIMARY KEY,
	    FK_MEDICO_FK_PESSOA_CPF varchar(45),
	    FK_HOSPITAL_cod_hospital int,
	    FK_DIAGNOSTICO_cod_diag int,
	    FK_PESSOA_CPF varchar(45),
	    hora_agenda time,
	    data_agenda date,
	    FK_STATUS_cod_status int
	);

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_2
	    FOREIGN KEY (FK_MEDICO_FK_PESSOA_CPF)
	    REFERENCES MEDICO (FK_PESSOA_CPF)
	    ON DELETE CASCADE;

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_3
	    FOREIGN KEY (FK_HOSPITAL_cod_hospital)
	    REFERENCES HOSPITAL (cod_hospital)
	    ON DELETE CASCADE;

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_4
	    FOREIGN KEY (FK_DIAGNOSTICO_cod_diag)
	    REFERENCES DIAGNOSTICO (cod_diag)
	    ON DELETE RESTRICT;

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_5
	    FOREIGN KEY (FK_PESSOA_CPF)
	    REFERENCES PESSOA (CPF)
	    ON DELETE CASCADE;

	ALTER TABLE CONSULTA ADD CONSTRAINT FK_CONSULTA_6
	    FOREIGN KEY (FK_STATUS_cod_status)
	    REFERENCES STATUS (cod_status)
	    ON DELETE CASCADE;

	INSERT INTO consulta (dt_consulta, hora, FK_STATUS_cod_status , cod_consulta, FK_PESSOA_CPF, FK_HOSPITAL_cod_hospital, 		FK_DIAGNOSTICO_cod_diag, FK_MEDICO_fk_pessoa_cpf, hora_agenda , data_agenda ) VALUES 
	('2018/01/12', '18:00', 1, 21,'456.654.654-00',10, 12, '345.543.897-00', '11:00', '2001/03/10'),
	('2018/08/23', '12:00', 1,  8, '456.654.654-00', 17, 80, '345.543.897-00', '12:00', '2002/04/11'),
	('2018/08/23', '13:00', 2,  9, '231.321.987-00',18,81, '123.321.789-00', '13:00', '2003/05/12'),
	('2018/03/09', '9:00', 1,  12, '231.321.987-00',12, 21, '123.321.789-00', '7:00', '2000/02/9'),
	('2018/05/13', '14:00', 1, 14, '145.541.789-00',21, 22,'123.321.789-00', '8:00', '2004/05/8'),
	('2018/04/11', '8:00', 2, 56, '145.541.789-00',53, 65, '231.321.987-00', '9:00', '2005/07/7'),
	('2018/04/11', '9:30', 1, 57, '345.543.897-00',13, 66, '231.321.987-00', '10:00', '2010/08/6'), 
	('2018/04/11', '7:00',  1, 34, '345.543.897-00',9, 43, '145.541.789-00', '14:00','2018/03/5'), 
	('2018/07/12', '8:00', 1, 77, '456.654.654-00',44, 47, '567.765.554-00', '15:00', '2017/02/4');


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
	

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/pessoainsert.png?raw=true "Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/consultainsert1.png?raw=true "Consulta-p1")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/consultainsert2.png?raw=true "Consulta-p2")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/hospitalinsert.png?raw=true "Hospital")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/diagnoitinsert.png?raw=true "Diagnostico")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/estadoinsert.png?raw=true "Estado")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/cidadeinsert.png?raw=true "Cidade")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/bairroinsert.png?raw=true "Bairro")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/complementoInsert.png?raw=true "Complemento")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/contato_pessoainsert.png?raw=true "Contato Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/contatoinsert.png?raw=true "Contato")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/convenioinsert.png?raw=true "Convênio")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/diag_doencainsert.png?raw=true "Diag-Doença")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/doencainsert.png?raw=true "Doença")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/lograEndinsert.png?raw=true "End-Logradouro")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/enderecoinsert.png?raw=true "Endereço")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/doencainsert.png?raw=true "Med-Especialidade")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/logradouroinsert.png?raw=true "Logradouro")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/med_pessoainsert.png?raw=true "Med-Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/medicoinsert.png?raw=true "Médico")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/doencainsert.png?raw=true "Alergia-Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/pessoa_cronicainsert.png?raw=true "DoençaC-Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/pessoaendinsert.png?raw=true "Endereço-Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/plan_pessoainsert.png?raw=true "PlanoS-Pessoa")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/sexoinsert.png?raw=true "Sexo")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/status.png?raw=true "Status")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/tp_sanguineoinsert.png?raw=true "Tipo Sanguíneo")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/trabalhainsert.png?raw=true "Trabalha")

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
    a) Criar outras 5 consultas que envolvam like ou ilike:
	select alergias from pessoa where alergias ilike '%e%';
	select nome from pessoa where nome like 'L%';
	select * from hospital where nome like 'S%';
	select * from diagnóstico where doença ilike '%l%';
	select receita from diagnóstico where receita like 'A%';
	
    b) Criar uma consulta para cada tipo de função data apresentada.
	select now();
	select current_date;
	select current_time;
	select age(current_date, ('2018/04/11'));
	select date_part('year',age(current_date, ('2018/04/11')));
	extract ('year' from ('2018/04/11'));

#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>
	drop table pessoa;
	drop table hospital;
	drop table consulta;
	alter table consulta drop hora;
	update consulta set cod_consulta = 7 where cod_consulta = 8;
	update pessoa set nome = João where nome = Leonardo;

#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        
	select cpf, nome, cod_consulta, cod_diagnostico, cod_hospital, nome_hospital, cod_bairro, nome_bairro, cod_cidade, nome_cidade, 	cod_estado, nome_estado  from estado
	inner JOIN cidade
	on (estado.cod_estado = cidade.fk_cod_estado)
	inner JOIN bairro
	on (cidade.cod_cidade = bairro.fk_cidade_cod_cidade)
	inner join pessoa
	on (bairro.cod_bairro = pessoa.fk_cod_bairro)
	inner JOIN hospital
	on (pessoa.cpf = hospital.fk_cpf)
	inner JOIN consulta
	on (hospital.cod_hospital = consulta.fk_cod_hospital)
	inner JOIN diagnostico
	on (consulta.fk_cod_diagnostico = diagnóstico.cod_diagnostico)

## Marco de Entrega 02 em: (16/06/2018)<br>
### ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO SEMESTRAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (30/06/2018)
<br>

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/group1.PNG?raw=true "Group1")
	
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/group2.png?raw=true "Group2")
	
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/group3.PNG?raw=true "Group3")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/group4.PNG?raw=true "Group4")

![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/group5.PNG?raw=true "Group5")
	
![Alt text](https://github.com/remedmax/trabalho01/blob/master/imagens/group6.PNG?raw=true "Group6")

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Não conseguimos identificar.
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
		
		1) 					
		create view nome_e_cpf_pessoa as	
		select nome,cpf
		from pessoa;
		select * from nome_e_cpf_pessoa;
		
		2)
		create view medic_pessoa as
		select nome,cpf from pessoa
		where cpf in (select cpf from medico);
		select * from medico_pessoa;
		
		3)
		create view quant_bairro as SELECT bairro.nome_bairro, count(hospital.fk_endereco_cod_endereco)
		FROM bairro 
		INNER JOIN endereco ON
		(bairro.cod_bairro = endereco.fk_bairro_cod_bairro)
		JOIN hospital ON
		(endereco.cod_endereco = hospital.fk_endereco_cod_endereco)
		WHERE endereco.cod_endereco in (select fk_endereco_cod_endereco from hospital)
		GROUP BY bairro.nome_bairro;
		select * from quant_bairro;
		
		4)
		create view cidade_bairro as
		select nome_cidade,cod_cidade from cidade
		where cod_cidade in (select FK_CIDADE_cod_cidade from bairro);
		select * from cidade_bairro;
		
		5)
		create view quant_consulta as SELECT hora, count(hora) AS quantidade
		FROM consulta
		GROUP BY hora
		ORDER BY count(consulta.fk_medico_fk_pessoa_cpf) DESC, hora ASC;
		select * from quant_consulta;
		
		6)
		create view plano_convenio as
		select num_carteirinha from plano_saude
		where num_carteirinha in (select FK_PLANO_SAUDE_num_carteirinha from convenio);
		select * from plano_convenio;

#### 9.10	SUBCONSULTAS (Mínimo 3)<br>
	select nome from pessoa 
	where cpf in (select cpf from medico);

	SELECT hospital.nome_hospital, count(consulta.fk_hospital_cod_hospital)
	FROM hospital inner join consulta on (consulta.fk_hospital_cod_hospital = hospital.cod_hospital)
	where consulta.fk_hospital_cod_hospital in(select distinct cod_hospital from hospital)
	GROUP BY hospital.nome_hospital;

	SELECT bairro.nome_bairro, count(hospital.fk_endereco_cod_endereco)
	FROM bairro 
	INNER JOIN endereco ON
	(bairro.cod_bairro = endereco.fk_bairro_cod_bairro)
	JOIN hospital ON
	(endereco.cod_endereco = hospital.fk_endereco_cod_endereco)
	WHERE endereco.cod_endereco in (select fk_endereco_cod_endereco from hospital)
	GROUP BY bairro.nome_bairro;

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


        
        


    





