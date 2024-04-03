O projeto "DesafioControleFluxo" consiste em um programa Java simples que permite ao usuário inserir dois números inteiros pelo terminal e, em seguida, realiza a contagem de 1 até a diferença entre esses dois números, imprimindo cada número no console. Este programa é composto por duas classes principais: Contador e ParametrosInvalidosException.

Classe Contador:

Esta classe contém o método main, que é o ponto de entrada do programa. Neste método, o usuário é solicitado a inserir dois números inteiros pelo terminal utilizando um objeto Scanner.
Os números inseridos são passados para o método contar, que realiza a lógica de contagem.
Dentro do bloco try-catch, qualquer exceção do tipo ParametrosInvalidosException é capturada e tratada. Se essa exceção for lançada, a mensagem "O segundo parâmetro deve ser maior que o primeiro" é exibida no console.


Classe ParametrosInvalidosException:

Esta classe é uma exceção customizada que estende a classe Exception.
Ela é usada para representar uma exceção específica que ocorre quando o segundo parâmetro inserido pelo usuário é menor ou igual ao primeiro parâmetro.
Quando instanciada com uma mensagem, essa exceção pode ser lançada no método contar para indicar que os parâmetros inseridos são inválidos.


Método contar:

Este método recebe dois parâmetros inteiros representando os números inseridos pelo usuário.
Ele verifica se o segundo parâmetro é maior que o primeiro. Se não for, lança uma exceção ParametrosInvalidosException.
Caso contrário, calcula a diferença entre os dois números e realiza um loop for para imprimir cada número incrementalmente no console.
Em resumo, o projeto permite ao usuário contar de um número até outro, desde que o segundo número seja maior que o primeiro. Se essa condição não for atendida, uma exceção é lançada e tratada, fornecendo uma mensagem informativa ao usuário.
