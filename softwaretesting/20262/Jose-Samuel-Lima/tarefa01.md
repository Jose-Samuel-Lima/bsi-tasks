# Tarefa 01 - Teste de Unidade, Integração, Cobertura e CI

**Nome:** José Samuel Lima
**GitHub:** [Jose-Samuel-Lima](https://github.com/Jose-Samuel-Lima)
**E-mail:** jose.lima.146@ufrn.edu.br
**Repositório do projeto:** [SpendSmart](https://github.com/MViniciusCoffe/SpendSmart)

## 1. Teste de Software

Teste de software é o processo utilizado para verificar se um sistema apresenta o comportamento esperado e para identificar erros durante o desenvolvimento. Os testes podem ser realizados em diferentes níveis, de acordo com a parte do sistema que está sendo avaliada.

O **teste de unidade** verifica uma pequena parte do sistema de forma isolada, normalmente uma função ou método. Seu objetivo é verificar se aquela unidade apresenta o resultado esperado para diferentes situações.

O **teste de integração** verifica a interação entre diferentes partes do sistema. Enquanto o teste de unidade procura avaliar componentes isoladamente, o teste de integração verifica se esses componentes conseguem trabalhar corretamente em conjunto.

Os testes são importantes porque ajudam a identificar problemas antes que o software seja utilizado pelos usuários, além de facilitar alterações e manutenção do sistema. No projeto SpendSmart, os testes serão utilizados principalmente para verificar as operações do CRUD e a integração entre seus componentes.


## 2. Linguagem e Stack

Para o desenvolvimento dos testes e evolução do projeto SpendSmart, será utilizada a linguagem **JavaScript**, já utilizada no projeto.

A aplicação utiliza **React** para a construção da interface e **Next.js** como framework da aplicação. Para realizar as requisições HTTP utilizadas nas operações do CRUD, o projeto utiliza a biblioteca **Axios**.

Para a implementação dos testes automatizados será utilizado o **Jest**, permitindo criar e executar testes para verificar o comportamento das funcionalidades do sistema.

### Stack utilizada

* **JavaScript:** linguagem de programação utilizada no projeto.
* **React:** biblioteca utilizada para construção da interface.
* **Next.js:** framework utilizado na aplicação.
* **Axios:** biblioteca utilizada para realizar requisições HTTP.
* **Jest:** framework que será utilizado para os testes automatizados.


## 3. Framework de Testes Unitários

O framework escolhido para os testes automatizados do projeto SpendSmart é o **Jest**.

O Jest é um framework de testes para JavaScript que permite criar, executar e verificar testes de forma automatizada. Ele possui recursos para realizar asserções com `expect`, organizar testes e criar funções simuladas (mocks), que serão utilizadas neste projeto para testar as operações do CRUD sem depender diretamente de serviços externos.

A documentação oficial do Jest apresenta exemplos de instalação utilizando npm, criação de arquivos de teste e configuração do script de testes no `package.json`.

No projeto SpendSmart, o Jest será utilizado para criar os testes unitários das operações do CRUD e, posteriormente, para executar os testes e gerar o relatório de cobertura.

**Documentação oficial:**
https://jestjs.io/docs/getting-started

**Documentação sobre mocks:**
https://jestjs.io/docs/mock-function-api


## 4. IDE e Ferramentas de Debug

A IDE utilizada no desenvolvimento do projeto SpendSmart é o **Visual Studio Code (VS Code)**.

O VS Code oferece recursos que auxiliam no desenvolvimento e na identificação de erros, como o **Debugger**, que permite executar o programa passo a passo, adicionar breakpoints, acompanhar valores das variáveis e analisar o fluxo de execução.

Além do debugger, o VS Code possui integração com o terminal, permitindo executar comandos do projeto, instalar dependências, executar os testes automatizados e analisar os resultados diretamente no ambiente de desenvolvimento.

No projeto SpendSmart, o VS Code será utilizado para desenvolver os testes com Jest, executar os testes e auxiliar na identificação de possíveis erros durante a implementação.

**Documentação oficial do Visual Studio Code sobre Debugging:**
https://code.visualstudio.com/docs/editor/debugging


## 5. Tutorial de CRUD com Testes

Foi pesquisado um projeto tutorial que apresenta a implementação de um CRUD utilizando **Express e Mongoose**, juntamente com testes unitários e testes de integração utilizando **Jest**.

O tutorial apresenta uma aplicação CRUD e demonstra como configurar o projeto, instalar as dependências, executar a aplicação e executar os testes. Também utiliza Jest para verificar o funcionamento das operações da aplicação.

Esse material é relacionado ao SpendSmart porque apresenta uma abordagem prática para testar operações de um CRUD, que será utilizada como referência para a implementação dos testes no projeto.

**Tutorial:**
https://github.com/minhajul-karim/crud-express-mongoose-with-unit-integration-tests

**Descrição:**
O projeto demonstra um CRUD desenvolvido com Express e Mongoose e possui testes unitários e de integração escritos com Jest. Ele será utilizado como referência para compreender a organização dos testes e a diferença entre testar componentes isoladamente e testar a integração entre partes da aplicação.


## 6. Mock Objects

**Mock Objects** são objetos simulados utilizados nos testes para representar o comportamento de componentes ou dependências reais. Eles permitem que uma parte do sistema seja testada de forma isolada, sem depender diretamente de serviços externos ou de outras partes da aplicação.

Os mocks são especialmente úteis em testes unitários porque permitem controlar o comportamento da dependência utilizada pelo código. Dessa forma, é possível definir previamente o resultado esperado e verificar se a unidade testada reage corretamente.

No projeto SpendSmart, os mocks serão utilizados principalmente para simular as requisições realizadas pelo **Axios**. Assim, os testes das operações do CRUD poderão verificar o comportamento das funções sem precisar realizar uma requisição real à API.

Por exemplo, em um teste de inserção de categoria, o Axios poderá ser simulado para retornar uma resposta de sucesso. O teste então verifica se a função do SpendSmart realizou a chamada esperada e tratou corretamente o resultado.

O uso de mocks permite, portanto, tornar os testes unitários mais rápidos, previsíveis e independentes de serviços externos.

**Referência:**
https://jestjs.io/docs/mock-function-api


## 7. Projeto CRUD

## 8. Testes e Cobertura

## 9. Integração Contínua (CI)

## 10. SonarQube
