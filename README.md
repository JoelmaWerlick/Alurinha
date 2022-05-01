# Alurinha
Repositorio criado para manusear o flexbox, que é uma expecificação de CSS.
A proposta do curso é o desenvolvimento do Alurinha, um gerenciador de cursos online.

## Quais as principais diferenças entre as nossas propriedades de posicionamento?

display: inline

Colocando display: inline nos elementos permite eles se posicionarem um do lado do outro, o problema do display: inline é que os elementos não aceitam mais que seja modificada tanto a width quanto a height. Isso limita MUITO nossas possibilidades.

display: inline-block

O display: inline-block permite os elementos se posicionarem um do lado do outro porém, diferentemente do display: inline ele permite que os elementos tenham sua width e height modificadas. Por esse motivo o display: inline-block é muito mais interessante na maioria dos casos do que o display: inline.

O problema de usar display: inline-block é espaçar os elementos entre si. Para fazer isso teríamos que colocar margins e fazer contas.

float: left | right

O float é mais complicado, ele empurra o elemento para um dos lados (left | right) e os elementos que estão embaixo sobem. Isso nem sempre é o que a gente quer. Além do mais o float não permite que usemos a propriedade vertical-align: middle para alinhar os elementos verticalmente. Ou seja, para contornar isso uma possibilidade seria ter que colocar margin-top ou bottom nos elementos e usar os temidos números mágicos!

display: flex

O display: flex veio com o intuito de facilitar nossa vida nesses aspectos de posicionamento. Ele permite os elementos ficarem um do lado do outro, permite espaçar os elementos de forma mais intuitiva e sem ter que fazer cálculos. Além disso ele também permite alinhar os elementos verticalmente de forma fácil.

O display flex pode ser um pouco mais complicado de usar tendo em vista que existem diversas propriedades que vem junto da especificação flexible box, todavia tudo isso foi feito para justamente melhorar nosso código.

## justify-content 

Colocar todo espaço à esquerda, jogando o conteúdo para direita com justify-content: flex-end.

Colocar todo espaço à direita, jogando o conteúdo para esquerda com justify-content: flex-start (que é o padrão).

Colocar todo espaço à esquerda e à direita, jogando o conteúdo para o meio com justify-content: center.

Colocar todo espaço entre os elementos como vimos antes usando justify-content: space-between.

E uma possibilidade bem interessante também é colocar o espaço em volta dos elementos. Podemos usar o justify-content: space-around para isso.

## align-items

flex-start: os itens são alinhados à parte superior do contêiner.
flex-end: os itens se alinham à parte inferior do contêiner.
center: os itens são alinhados no centro vertical do contêiner.
baseline: os itens são exibidos na linha de base do contêiner.
stretch: Os itens são esticados para caber no contêiner.

## flex-direction

row: Os itens são colocados da mesma forma que a direção do texto.
row-reverse: Os itens são colocados em oposição à direção do texto.
column: Os itens são colocados de cima para baixo.
column-reverse: Os itens são colocados de baixo para cima.

## Flex container e flex items

Quando colocamos display: flex em um elemento, o navegador passa a considerar esse elemento como um flex container, ou seja, cria todo aquele comportamento que vimos anteriormente no curso, os filhos ficam um do lado do outro e podemos aplicar propriedades para espaçá-los.

Os filhos de um flex container por sua vez também ganham um nome, são chamados de flex items.

Quando utilizamos flexbox temos que ficar atentos em quem colocamos as propriedades de espaçamento e distribuição do flex. Por exemplo, existem algumas propriedades que devem ser aplicadas à flex container e outras que devem ser aplicadas nos flex items.

![mThvRZq](https://user-images.githubusercontent.com/100633937/166129111-8137624d-fdfb-4a00-8643-905c5108dca5.png)

container:

display: flex
flex-direction
justify-content
flex-wrap
flex-flow
align-items
align-content

flex item:

order
flex-grow
flex-shrink
flex-basis
flex
align-self

[FlexFrog] http://flexboxfroggy.com/

![5_8+mostrando+o+flexbox+froggy](https://user-images.githubusercontent.com/100633937/166129179-5f8ee470-361b-43f4-9785-8fec13c7c317.png)


