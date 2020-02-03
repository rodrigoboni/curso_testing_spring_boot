# curso_testing_spring_boot
Conteúdo curso Udemy Testing Spring Boot

# Porque testar ?
* Possuir testes bem definidos no seu projeto permite realizar alterações com segurança e confiança, pois os testes vão apontar o que mudou
* Aumenta e garante a qualidade do código / do software
* Padrão amplamente aceito e requerido

# Termos
* test fixture - conjunto de códigos usados como base para testes (definindo mocks por exemplo, dados de entrada, simulando banco de dados etc)
* unit tests - código escrito p/ testar código, testar partes específicas do código
* code coverage - quanto mais linhas / trechos de código forem cobertos por testes unitários maior o % de coverage - recomendado no mínimo 70% de cobertura - o % ideal varia de acordo com o projeto

# Testes unitários
* específicos / para testar trecho / funcionalidade
* tem que serem pequenos e rápidos de executar
* sem dependências externas p/ executar
* é o menor escopo de teste

# Testes de integração
* visa testar integração / comportamento entre componentes do projeto
* mais lento que testes unitários
* escopo maior do que teste unitário

# Testes funcionais
* visa testar projeto em ambiente conhecido
* geralmente utiliza ferramentas como selenium para simular usuário no front end, faz chamadas a api's, recebe e envia mensagens assíncronas etc
* nível mais alto de teste
* tipo de testes mais lento

# Recomendação de testes x tipo de teste:
* testes unitários devem ser a maioria - testam funcionalidades específicas, são rápidos de executar, aumentam % coverage
* testes de integração - após testar as funcionalidades isoladamente é recomendado testar a integração entre as funcionalidades (testes deste tipo devem ser em menor número que os unitários, por serem mais lentos)
* testes funcionais - último tipo de teste a ser aplicado, em menor escala, devido aos requisitos para implementar e pelo maior tempo necessário para executar, além de ser necessário o ambiente para o teste. 

# Técnicas de teste:
* TDD - primeiro teste, depois implemente (focado em funcionadlidade)
* BDD - semelhante ao tdd, porém focado no comportamento 

# Componentes de teste:
* Mock - implementação falsa de um objeto (de uma entidade no bd por ex)
* Spy - utiliza o objeto real, porém "empacotado", p/ sobrepor algum comportamento / resposta

# Frameworks de teste:
* JUnit 5
* Spock - framework BDD - utiliza groovy
* cucumber - framework BDD - utilizar síntaxe gherkin p/ descrever os cenários
* mockito - focado em mocks - utilizado em conjunto com frameworks de teste
* spring mvc test - módulo de testes nativo do framework spring - focado mais em controllers mvc
* rest-assured - focado em testar apis rest
* selenium - automação do web browser - utilizado em conjunto com outros frameworks, como junit
* geb - framework feito sobre o selenium

# CI / CD
* Utilizar CI é importante para melhorar / garantir a qualidade do código, pois é uma base comum de código onde todos mesclam seus ajustes e uma pipeline de build é executada, com testes, e qdo um teste falha o deploy é interrompido, alertando para problemas.

# TDD
* projeto tdd-by-example
* https://github.com/springframeworkguru/tdd-by-example