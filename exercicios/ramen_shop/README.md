# Ramen Shop com padrões de projeto

**Professor**: Hugo de Paula

* * *

## Objetivo

O objetivo deste trabalho é construir um programa coeso e extensível, que utilize padrões de projeto.

## Contextualização

Um izakaya é um bar japonês informal que serve comida e bebidas, sendo uma opção popular para jantares após o trabalho. 

Os izakayas são locais pequenos e simples, onde se pode encontrar cerveja gelada, destilados, refrigerantes e uma variedade de comida para partilhar. 


Os izakayas são conhecidos por oferecer pratos quentinhos e saborosos para petiscar, como tsukemonos (conservas), takoyakis (bolinhos de polvo), karaague (frango frito), berinjela com missô, oniguiri, bardana e panceta picante. 

Um tipo de izakaya muito comum é o **Ramen Shop**, especializado em vender o macarrão tipo *Lámen*, conhecido no Brasil pelo Miojo da Nissin.


![Ichiran Ramen Shop em Osaka, Japão.](osaka-japan-november-ichiran-ramen-japanese-ramen.jpg)

A Figura mostra o *Ichiran Ramen Shop* em Osaka, no Japão. A máquina exposta na calçada permite ao cliente escolher o prato que deseja. Ele recebe uma senha e busca o prato quando estiver pronto.

## Requisitos do problema

Você deverá desenvolver um sistema para um **Ramen Shop**. A seguir é apresentado o menu que deve ser implementado.

* * *

**RAMEN SHOP MENU**

| TAMANHO |   PREÇO  |   | PROTEÍNA |   PREÇO   |
|---------|----------|---|----------|-----------|
| Pequeno | R$ 9,90  |   | Vegano   | + R$ 3,90 |
| Médio   | R$ 12,90 |   | Boi      | + R$ 7,90 |
| Grande  | R$ 15,90 |   | Porco    | + R$ 5,90 |

|    ACRÉSCIMO    |    PREÇO   |   | ACRÉSCIMO  |  PREÇO    |
|-----------------|------------|---|------------|-----------|
| Proteína Extra  |  + R$ 4,00 |   | Chilli     | + R$ 2,50 |
| Crème Alho      |  + R$ 1,50 |   | Croutons   | + R$ 2,00 |
| Shitake         |  + R$ 6,90 |   | Tofu       | + R$ 2,70 |


|   BEBIDAS       |    PREÇO   | 
|-----------------|------------|
| Refrigerante    |  R$ 5,90   |
| O-Cha (Verde)   |  R$ 3,90   |
| Ko-Cha (Preto)  |  R$ 0,00   |

* * *

O cliente escolhe o tamanho do prato, que possui um preço base. A cada adicional no "Combo", o preço é acrescido. Ao terminar a escolha, o sistema calcula o total e emite o número do pedido.

O pedido é então adicionado a uma lista de espera e encaminhado à cozinha, que irá fabricar o prato do pedido. Quando o pedido estiver pronto, o cliente deve ser notificado. Após marcar o pedido como retirado, ele vai para o balanço final do restaurante.

O sistema deve garantir que exista uma única lista de espera no restaurante. Não pode haver listas paralelas.

O balanço final do restaurante deve exibir uma lista dos pedidos realizados, a quantidade de pedidos, a receita total e o ticket médio de cada pedido.

## Requisitos não funcionais

O trabalho deverá utilizar pelo menos três dos seguintes padrões de projeto: **Singleton**, **Decorator**, **Factory** e **Observer**.

- Construa o diagrama UML da solução.
- Implemente os construtores com parâmetros para todas as classes.
- Implemente os *getters/setters* para os atributos pertinentes.
- Adicione os atributos adicionais sejam porventura necessários.
- Parametrize o código para evitar repetição e aumentar a legibilidade.
- Utilize estruturas de dados baseada em Collections e Streams.
- Utilizando a JUnit, construa os testes unitários necessários para testar os valores dos atributos de todas as classes.
- Certifique-se de que seu código seja eficiente e modular.
- Utilize boas práticas de programação e comente seu código conforme necessário para facilitar a compreensão.

## Entrega

Entregue o trabalho no Github Classroom.

Utilize a ferramenta Maven para construir o projeto: group ID **br.lpm** e Artifact ID: **ramen\_shop**

A maneira correta de fazer isso é a seguinte:

1. Acesse o **Assignment** do **Github Classroom** para criar seu repositório para o exercício.
2. Realize a clonagem do repositório para a sua máquina local.
3. Crie o projeto Maven dentro do seu repositório.
4. Desenvolva o trabalho realizando commits a cada requisito implementado. Use commits pequenos para armazenar a evolução do seu trabalho.
5. Realize o push dos commits para o repositório remoto.