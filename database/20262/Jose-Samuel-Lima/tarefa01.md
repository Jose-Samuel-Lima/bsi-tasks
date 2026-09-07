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

Q3. Explique as propriedades ACID: atomicidade, consistência, isolamento e durabilidade. Para cada propriedade, descreva um exemplo prático no contexto de uma transferência bancária e explique o que aconteceria se o SGBD não garantisse essa propriedade.

Atomicidade:

A atomicidade determina que uma transação deve ser executada completamente ou não ser executada. Não deve existir um estado em que apenas parte da operação tenha sido realizada.

Exemplo: em uma transferência bancária de R$ 500,00, o sistema precisa retirar R$ 500,00 da conta de origem e adicionar R$ 500,00 à conta de destino.

Se a atomicidade não fosse garantida e o sistema sofresse uma falha depois de debitar a conta de origem, mas antes de creditar a conta de destino, o dinheiro poderia desaparecer da conta de origem sem aparecer na conta de destino.

Consistência:

A consistência garante que uma transação leve o banco de dados de um estado válido para outro estado válido, respeitando todas as regras e restrições definidas.

Exemplo: se uma conta possui R$ 1.000,00 e uma transferência de R$ 500,00 é realizada, após a operação o saldo deve ser R$ 500,00, respeitando as regras do banco.

Se a consistência não fosse garantida, uma transação poderia deixar dados inválidos, como um saldo incorreto ou uma operação que viole uma regra estabelecida pelo banco.

Isolamento:

O isolamento garante que transações executadas simultaneamente não interfiram de maneira incorreta umas nas outras. Cada transação deve funcionar como se estivesse sendo executada de forma independente.

Exemplo: duas operações tentam realizar transferências simultaneamente usando o mesmo saldo de uma conta.

Se o isolamento não fosse garantido, as duas operações poderiam ler o mesmo saldo antes que uma delas fosse atualizada, causando cálculos incorretos e podendo permitir que o banco registrasse operações incompatíveis com o saldo disponível.

Durabilidade:

A durabilidade garante que, depois que uma transação for confirmada, suas alterações permaneçam armazenadas mesmo que ocorra uma falha no sistema.

Exemplo: depois que uma transferência bancária é confirmada, os novos saldos devem permanecer registrados.

Se a durabilidade não fosse garantida e o servidor sofresse uma falha logo após confirmar a transferência, as alterações poderiam ser perdidas e o sistema poderia retornar aos saldos anteriores.