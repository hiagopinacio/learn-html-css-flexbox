# Flexbox

## Quais as principais diferenças entre as nossas propriedades de posicionamento?

### `display: inline`

Colocando display: inline nos elementos permite eles se posicionarem um do lado do outro, o problema do display: inline é que os elementos não aceitam mais que seja modificada tanto a width quanto a height. Isso limita MUITO nossas possibilidades.
    
### `display: inline-block`

O display: inline-block permite os elementos se posicionarem um do lado do outro porém, diferentemente do display: inline ele permite que os elementos tenham sua width e height modificadas. Por esse motivo o display: inline-block é muito mais interessante na maioria dos casos do que o display: inline.

O problema de usar display: inline-block é espaçar os elementos entre si. Para fazer isso teríamos que colocar margins e fazer contas.

### `float: left | right`

O float é mais complicado, ele empurra o elemento para um dos lados (left | right) e os elementos que estão embaixo sobem. Isso nem sempre é o que a gente quer. Além do mais o float não permite que usemos a propriedade vertical-align: middle para alinhar os elementos verticalmente. Ou seja, para contornar isso uma possibilidade seria ter que colocar margin-top ou bottom nos elementos e usar os temidos números mágicos!

### `display: flex`

O display: flex veio com o intuito de facilitar nossa vida nesses aspectos de posicionamento. Ele permite os elementos ficarem um do lado do outro, permite espaçar os elementos de forma mais intuitiva e sem ter que fazer cálculos. Além disso ele também permite alinhar os elementos verticalmente de forma fácil.

O display flex pode ser um pouco mais complicado de usar tendo em vista que existem diversas propriedades que vem junto da especificação flexible box, todavia tudo isso foi feito para justamente melhorar nosso código.

Agora que já tivemos essa introdução, vamos logo começar a organizar nosso site com flex (;

---
## Aula 1 -  Utilizando o Flex

Para aplicar o flex nos elementos de um container, devemos aplicar a propriedade `display:flex` no cointeiner pai.

Podemos alinhar verticalmente os elementos adicionado `align-items: center;`.

Por fim podemos justificar os elementos dentro do container com `justify-content`. Para adicionar um espaçamento igual entre os elementos de um container com tamanho definido, podemos utilizar o parâmetro `space-between`.

Ex. de aplicação destas 3 propriedades css na classe pai:

```css
.pai {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```

---
## Aula 2 - Fazendo o footer e controlando melhor os elementos