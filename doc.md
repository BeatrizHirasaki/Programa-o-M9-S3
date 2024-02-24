# Relatório sobre a Criação de um Projeto e Teste de Unidade em C#

## Introdução

Este relatório descreve a tecnologia e os conceitos aprendidos a partir de um artigo sobre a criação de um projeto de aplicativo de console em C# utilizando o Visual Studio e a implementação de testes de unidade utilizando o MSTest.

## Criação do Projeto

O processo começa com a criação de um novo projeto de Aplicativo de Console em C# para .NET no Visual Studio. O projeto é nomeado `Bank`, e é recomendado usar a estrutura de destino .NET 8. O projeto é configurado com um arquivo `Program.cs`, que é substituído por uma classe `BankAccount` demonstrando funcionalidades básicas de uma conta bancária, incluindo operações de débito e crédito.

## Estrutura da Classe `BankAccount`

A classe `BankAccount` inclui métodos para debitar e creditar a conta, além de propriedades para o nome do cliente e o saldo atual. O método `Debit` lança uma exceção `ArgumentOutOfRangeException` se o valor do débito for maior que o saldo ou negativo. De forma similar, o método `Credit` só permite valores positivos. Um método `Main` é incluído para demonstrar o uso da classe.

## Criação do Projeto de Teste de Unidade

Após a criação do projeto principal, um projeto de teste de unidade é adicionado à solução. O projeto de teste, chamado `BankTests`, utiliza o MSTest para verificar o comportamento da classe `BankAccount`, focando especialmente no método `Debit`.

## Classe de Teste `BankAccountTests`

Dentro do projeto de teste, uma classe `BankAccountTests` é criada para implementar os testes de unidade. Os testes verificam se a classe `BankAccount` se comporta conforme esperado em diferentes cenários, como débitos válidos, tentativas de débito com valores negativos ou superiores ao saldo atual.

## Principais Conceitos Aprendidos

- **Criação de Projetos no Visual Studio:** Aprendi a iniciar projetos de aplicativo de console e de teste de unidade, configurando-os adequadamente para o desenvolvimento.
- **Estrutura e Funcionalidades Básicas de Classes em C#:** A classe `BankAccount` serviu como um bom exemplo prático do uso de propriedades, construtores e exceções em C#.
- **Testes de Unidade com MSTest:** Aprendi como funcionam os testes, por meio da demonstração de como criar e executar testes de unidade para validar o comportamento esperado de métodos específicos, utilizando asserções para verificar os resultados.
- **Refatoração Baseada em Testes:** O artigo ensinou também como os testes de unidade podem revelar bugs e guiar a refatoração do código para melhorar sua qualidade e robustez.

## Conclusão

O processo descrito no artigo proporciona uma introdução prática ao desenvolvimento em C# com o Visual Studio, cobrindo desde a criação de um projeto simples até a implementação e execução de testes de unidade. Através deste exercício, pude compreender a importância dos testes de unidade para a validação e melhoria contínua do código.
