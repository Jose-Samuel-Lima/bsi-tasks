Tarefa 01 - Conceitos de BD, ACID e SGBD

Q1. Descreva o que é um Banco de Dados e o que é um Sistema Gerenciador de Banco de Dados. Cite exemplos de Bancos de Dados e seus SGBDs.

Um Banco de Dados (BD) é uma coleção organizada de dados relacionados, armazenados de forma que possam ser consultados, inseridos, alterados e removidos de maneira eficiente. Ele permite armazenar informações de forma estruturada para que possam ser utilizadas por sistemas e usuários.
Um Sistema Gerenciador de Banco de Dados (SGBD) é o software responsável por criar, organizar, armazenar, consultar e controlar o acesso aos dados de um banco de dados. Além disso, o SGBD oferece mecanismos para garantir segurança, integridade, controle de concorrência, recuperação de falhas e consistência dos dados.

Exemplos de bancos de dados e seus SGBD:

Banco de Dados	            |  SGBD
Banco de dados relacional	|  MySQL
Banco de dados relacional   |  PostgreSQL
Banco de dados corporativo  |  Oracle Database
Banco de dados corporativo  |  SQL Server
Banco de dados embutido	    |  SQLite
Banco de dados orientado a documentos  |  MongoDB

Q2. Quais os principais problemas de utilizar Sistemas de Arquivos para armazenagem de dados?

Um dos principais problemas é a redundância de dados, pois a mesma informação pode ser armazenada em vários arquivos diferentes. Isso aumenta o espaço utilizado e pode fazer com que existam versões diferentes da mesma informação.

Outro problema é a inconsistência dos dados. Quando uma informação é alterada em um arquivo, mas não é atualizada em outro, os arquivos podem apresentar informações diferentes sobre o mesmo objeto.

Também existe dificuldade para realizar consultas complexas. Em sistemas de arquivos, muitas consultas exigem que a aplicação seja responsável por localizar e processar os dados manualmente.

Outro problema é o controle de acesso e segurança. É mais difícil controlar quais usuários podem visualizar ou alterar determinadas informações quando os dados estão espalhados em vários arquivos.

Os sistemas de arquivos também apresentam dificuldades relacionadas à concorrência, pois vários usuários ou programas podem tentar alterar o mesmo arquivo simultaneamente, causando conflitos ou perda de informações.

Além disso, a recuperação após falhas pode ser limitada. Uma falha de energia ou do sistema durante uma alteração pode deixar os arquivos em um estado incompleto ou inconsistente.