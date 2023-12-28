# 🚀 Decola Tech 2024 - Orientação a Objetos com C#
www.dio.me

## 🌟 Desafio de projeto III - Implementanto validações de testes unitários com C#
Este é o terceiro desafio de projeto do Bootcamp Decola Tech 2024, sendo feito durante o módulo de Orientação a Objetos com C#. Para este projeto, desenvolvi os requisitos solicitados e obrigatórios para o desafio, deixando em aberto por ser a versão 1.0. Pretendo, conforme avanço no conhecimento da linguagem, aprimorá-lo num futuro próximo.

## ❓ Contexto
Foi disponibilizado um projeto base console com duas classes (ValidacoesLista e ValidacoesString, cada qual com seus respectivos métodos prontos) e um projeto do tipo testes, também com duas classes (ValidacoesListaTests e ValidacoesStringTests). No projeto de testes, temos alguns trechos de código faltando ou incorretos. A ideia foi, portanto, consertar esse código de forma que o teste fosse feito de forma correta, possibilitando uma apropriada verificação e validação das alterações realizadas.

## 📌 Premissas
O sistema hoje possui dois projetos: um do tipo console, e um do tipo testes com **xUnit**. O projeto do tipo console possui duas classes em que são realizadas as lógicas principais: **ValidacoesLista** e **ValidacoesString**. Essas classes contém métodos em comum que são usados para realizar diversas validações em determinados cenários.

O projeto de testes possui as classes de teste **ValidacoesListaTests** e **ValidacoesStringTests**, assim como seus métodos para validar o projeto do tipo console, porém estão incompletos. 

O seu objetivo é implementar os métodos de testes contidos no projeto.

## ❗Projeto Console, suas classes e métodos

Essas são as classes do projeto console, onde fica a principal lógica do sistema.

**Classe ValidaçõesLista**

Classe responsável por realizar diversas validações envolvendo listas.

| Classe          | Método                       | Objetivo                                                                                                                |
|---------------- |------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| ValidacoesLista | RemoverNumerosNegativos      | Recebe uma lista de números inteiros e retorna uma nova lista, apenas com os números positivos                          |
| ValidacoesLista | ListaContemDeterminadoNumero | Recebe uma lista de números inteiros e verifica se um determinado número está presente dentro dessa lista               |
| ValidacoesLista | MultiplicarNumerosLista      | Recebe uma lista de números inteiros e retorna uma nova lista, com seus valores múltiplicados por um determinado número |
| ValidacoesLista | RetornarMaiorNumeroLista     | Recebe uma lista de números inteiros e retorna o maior número entre eles                                                |
| ValidacoesLista | RetornarMenorNumeroLista     | Recebe uma lista de números inteiros e retorna o menor número entre eles                                                |

**Classe ValidacoesString**

Classe responsável por realizar diversas validações envolvendo strings.

| Classe           | Método                       | Objetivo                                                                                                                
|------------------|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ValidacoesString | RetornarQuantidadeCaracteres | Recebe um texto qualquer e retorna a quantidade de caracteres presentes no texto                                                                           |
| ValidacoesString | ContemCaractere              | Recebe um texto qualquer e um texto a ser procurado, retorna verdadeiro ou falso se um determinado trecho procurado está presente no texto                 |
| ValidacoesString | TextoTerminaCom              | Recebe um texto qualquer e um trecho a ser procurado, retorna verdadeiro ou falso se um determinado trecho procurado está presente no final do texto apenas |

## ‼️ Projeto do tipo teste, suas classes e métodos

**Classe ValidacoesListaTests**

Classe responsável por realizar os testes da classe ValidacoesLista.

| Classe               | Método de teste                               | Resultado esperado do teste
|----------------------|-----------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| ValidacoesListaTests | DeveRemoverNumerosNegativosDeUmaLista         | Ao passar uma lista com diversos números, incluindo positivos e negativos, deve ser retornado uma nova lista apenas com números positivos  |
| ValidacoesListaTests | DeveConterONumero9NaLista                     | Ao passar uma lista com diversos números, incluindo o número 9, deve retornar verdadeiro, pois encontrou o 9 na lista                      |
| ValidacoesListaTests | NaoDeveConterONumero10NaLista                 | Ao passar uma lista com diversos números, mas sem o número 10, deve retornar falso, pois não encontrou o 10 na lista                       |
| ValidacoesListaTests | DeveMultiplicarOsElementosDaListaPor2         | Ao passar uma lista de inteiros, deve retornar uma nova lista, com todos os elementos da lista multiplicados por 2                         |
| ValidacoesListaTests | DeveRetornar9ComoMaiorNumeroDaLista           | Ao passar uma lista de números inteiros, sendo o maior deles 9, deve retornar o 9 como maior elemento dentro dessa lista                   |
| ValidacoesListaTests | DeveRetornarOitoNegativoComoMenorNumeroDaList | Ao passar uma lista de números inteiros, sendo o menor deles -8, deve retornar o -8 como menor elemento dentro dessa lista                 |

**Classe ValidacoesStringTests**

Classe responsável por realizar os testes da classe ValidacoesString.

| Classe                | Método de teste                                  | Resultado esperado do teste
|---------------------- |--------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ValidacoesStringTests | DeveRetornar6QuantidadeCaracteresDaPalavraMatrix | Ao passar um texto escrito a palavra "Matrix", deve retornar o número 6, representando 6 caracteres presentes na palavra                                                                         |
| ValidacoesStringTests | DeveContemAPalavraQualquerNoTexto                | Ao passar um texto escrito "Esse é um texto qualquer" e procurar pela palavra "qualquer", deve retornar verdadeiro pois a palavra existe no texto                                                |
| ValidacoesStringTests | NaoDeveConterAPalavraTesteNoTexto                | Ao passar um texto escrito "Esse é um texto qualquer" e procurar pela palavra "teste", deve retornar falso pois a palavra não existe no texto                                                    |
| ValidacoesStringTests | TextoDeveTerminarComAPalavraProcurado            | Ao passar um texto escrito "Começo, meio e fim do texto procurado" e procurar pela palavra "procurado", deve retornar verdadeiro pois a palavra existe no texto e está inclusa no final do texto |

## ⚙️ Estrutura do projeto

O projeto está estruturado da seguinte maneira:

![Métodos Swagger](Imagens/projeto.png)


## 💡 Solução
O código de testes está pela metade, e você deverá dar continuidade implementando os testes descritos acima, para que no final, tenhamos um programa de testes funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima.

## 💻 Saída

![image](https://github.com/tainasays/decolaTech4-desafio-projeto3/assets/102188509/088d6377-38d2-4aaa-b651-ac9633c7f8c2)

### 🔧 Código

* [Services: ValidacoesLista.cs](https://github.com/tainasays/decolaTech4-desafio-projeto3/blob/main/TestesUnitarios.Desafio.Console/Services/ValidacoesLista.cs)
* [Services: ValidacoesString.cs](https://github.com/tainasays/decolaTech4-desafio-projeto3/blob/main/TestesUnitarios.Desafio.Console/Services/ValidacoesString.cs)
* [Testes: ValidacoesListaTests.cs](https://github.com/tainasays/decolaTech4-desafio-projeto3/blob/main/TestesUnitarios.Desafio.Tests/ValidacoesListaTests.cs)
* [Testes: ValidacoesStringTests.cs](https://github.com/tainasays/decolaTech4-desafio-projeto3/blob/main/TestesUnitarios.Desafio.Tests/ValidacoesStringTests.cs)
  
