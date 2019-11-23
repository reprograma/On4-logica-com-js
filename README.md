# Lógica

## Objetivo
Entender os princípios básicos de lógica de programação utilizando a linguagem JavaScript

## Porque aprender lógica com Javascript
> JavaScript pode ser a linguagem ideal para quem quer aprender a programar. No JavaScript todo o processo de configuração de ambiente é minimizado. Isso não parece grande vantagem, mas você pode repetir o feito em casa, em um computador diferente, com outro browser e sistema operacional - [Paulo Silveira](https://blog.caelum.com.br/comecar-a-programar-e-com-javascript/)

Recursos necessários para esta aula - navegador e editor de texto 

## Console

O objeto Console fornece acesso ao console de depuração do navegador. O seu funcionamento específico varia de navegador para navegador, mas existe um conjunto de ferramentas que na prática são fornecidas normalmente.

Com o navegador aberto como abrir o painel dedicado Console:
- Pressione F12 ou fn+F12, se o DevTools não estiver aberto no console pressione o botão do Console.
- Pressione Ctrl+Shift+J (Windows/Linux) ou Cmd+Opt+J (Mac)
- Clique com o botão direito do mouse em uma página web qualquer e clique na opção Inspecionar/Inspect, se o DevTools não estiver aberto no console pressione o botão do Console.

Essa tela deve aparecer.

<img src="https://developers.google.com/web/tools/chrome-devtools/console/images/console-panel.png?hl=pt-br">

> Mais: Prompt e alert!

---

## Chamar o JS dentro do HTML

Você precisa avisar ao navegador que existe um arquivo Javascipt e que ele precisa carregá-lo.

``` javascript
<script src="./js/hello.js"></script>`
```

```javascript
<script>
    Seu script
    Essa não é uma boa prática, serve apenas para exercícios e pequenos testes.
</script>
```
---

## O que é um algoritmo
> [Ada Lovelace, a primeira programadora de todos os tempos](https://canaltech.com.br/curiosidades/mulheres-historicas-ada-lovelace-a-primeira-programadora-de-todos-os-tempos-71395/)

**Algoritmo é uma "receita"** para executarmos uma tarefa ou resolver algum problema. Utilizamos algoritmos no nosso dia-a-dia para a execução de alguma tarefa ou até mesmo resolver algum problema.

Para fazer um computador fazer qualquer coisa, você precisa escrever um programa de computador. Para escrever um programa de computador, você tem que dizer ao computador, passo a passo, exatamente o que você quer que ele faça. O computador "executa" o programa, seguindo cada etapa mecanicamente, para atingir o objetivo final.

**Alguns exemplos de algoritmos que podemos citar: receitas culinárias, manual de instrução de aparelhos e funções matemáticas.**

Pense na receita culinária, por exemplo. Ela tem os ingredientes necessários **(dados de entrada)**, passo a passo para realizar a receita **(processamento ou instruções lógicas)** e o prato finalizado **(saída esperada)**. 

Um algoritmo, portanto, conta com a entrada (input), com o processamento desses dados e saída (output) de informações.

As estruturas de um algoritmo são:

- **variáveis**: são as informações de entrada inseridas que determinam aonde o algoritmo poderá ir. As mais comuns são texto, inteiro, lógico e real;
- **comandos de repetição***: consiste no uso de “se” e “enquanto”, para que o algoritmo saiba o que fazer quando determinados processos ocorrerem e o que fazer se eles mudarem.

<img src="assets/flow-2.png">

## Variáveis e constantes

O recurso utilizado nos programas para escrever e **ler dados da memória do computador** é conhecido como variável, que é simplesmente um espaço na memória o qual reservamos e damos um nome. Por exemplo, podemos criar uma variável chamada "idade" para armazenar a idade de uma pessoa. Você pode imaginar uma variável como uma gaveta "etiquetada" em um armário.

<img src="assets/var.png">

Toda vez que precisarmos armezanar e recuperar dados utilizaremos variáveis.

No Javascript temos 3 maneiras de usar variáveis:
- var (no console vamos usar essa)
- let
- const 

```javascript
var numero = 1
var texto = "Javascript!!!"
```

Declarando variáveis

Um identificador JavaScript deve começar com: 
- uma letra
- underline (_)
- cifrão ($)

Os caracteres subsequentes podem também ser 
- números (0-9)
- letras incluem caracteres de "A" a "Z" (maiúsculos)
- caracteres de "a" a "z" (minúsculos)

Uma varivável não pode ser uma palavra reservada, [clique aqui para saber quais são:](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords)


## Tipos de dados

### String
é uma sequência de caracteres usados para representar texto.

```javascript
"Variáveis em Javascript são uma forma para se salvar dados"
"Isabelle"
"1 é um número ímpar"
```

### Number
é um tipo de dado numérico. 

```javascript
1
20
300
4000
94863049863409863
```

### Boolean
é um tipo de dado lógico que pode ter apenas um de dois valores possíveis: verdadeiro ou falso. 

```javascript
false
true
```

### Null
representa um valor nulo ou "vazio".

```javascript
null
```

```javascript
var y = null;
console.log(y)
```

### undefined

```javascript
undefined
```

```javascript
var x;
console.log(x)
```

O javascript não tem o que chamamos de tipagem de dados que é literalmente descrever qual é o tipo dessa variável, o que ele faz é "entender/adivinhar" qual é o tipo de dados de determinada variável sem ela ter sido declarada no código escrito.

----
## Ferramentas para interagir com os inputs

O `alert` mostra uma mensagem na tela como um pop-up.

```javascript
let mensagem = 'Mensagem que vai aparecer no nosso alerta';
alert(mensagem);

```
O `confirm` é um pop-up que oferece uma lógica através de dois botões - o Ok (true) e o Cancel (false)
```javascript
let mensagem = 'Aperte o botão ok';
confirm(mensagem);
// Se o usuário apertar Ok vai retornar true, se apertar Cancel vai retornar false
```

O `prompt` é um pop-up que nos oferece um input para coletarmos variáveis.

```javascript
let nome = 'Digite o seu nome';
prompt(nome);
```

----
Vamos aos programas e aos processamentos de dados

----

## Operadores 

### Operadores de atribuição
O operador de atribuição básico é o igual (=), que atribui o valor do operando à direita ao operando à esquerda. Isto é, x = y atribui o valor de y a x.

#### Igual
```javascript
var y = 7;
var x = y; // x é igual à 7
```

### Operadores Aritméticos

#### Adição (+)

```javascript
var y = 7;
var x = 3;
var resultado = y + x 
console.log(resultado) // 10
```

#### Subtração (-)

```javascript
var y = 5;
var x = 2;
var resultado = y - x 
console.log(resultado) // 3
```

#### Multiplicação(*)

```javascript
var y = 4;
var x = 5;
var resultado = y * x 
console.log(resultado) // 20
```

#### Divisão (/) 
O operador de divisão produz o quociente de seus operandos onde o operando da esquerda é o dividendo e o da direita é o divisor.


```javascript
var y = 10;
var x = 2;
var resultado = y / x 
console.log(resultado) // 5
```

#### Módulo (%)
O operador módulo retorna o resto inteiro da divisão de um numero pelo outro.

```javascript
var y = 10;
var x = 2;
var resultado = y % x 
console.log(resultado) // 0
```

<!-- incremento (++)
decremento (--)
expoente (**)

abreviados
+=
-=
*= 
/=  -->
### Operadores de Comparação - Relacional e Igualdade

#### == Igual 
Retorna verdadeiro caso os operandos sejam iguais.	

```javascript
3 == var1
"3" == var1
3 == '3'
```

#### != Não igual	
Retorna verdadeiro caso os operandos não sejam iguais.	

```javascript
var1 != 4
var2 != "3"
```
#### === Estritamente igual 
Retorna verdadeiro caso os operandos sejam iguais e do mesmo tipo. Veja também Object.is e igualdade em JS.

```javascript
3 === var1
```

#### !== Estritamente não igual 
Retorna verdadeiro caso os operandos não sejam iguais e/ou não sejam do mesmo tipo.

```javascript
var1 !== "3"
3 !== '3'
```
#### > maior que
O operador de Maior retorna true se o operando da esquerda for maior que o operando da direita.

```javascript
4 > 3 // true
```

#### >= maior ou igual a
O operador maior ou igual retorna true se o operando da esquerda for maior ou igual ao operando da direita.

```javascript
4 >= 3 // true
3 >= 3 // true
```

#### < menor que
O operador menor retorna true (verdadeiro) se o operando da esquerda for menor que o operando da direita.

```javascript
3 < 4 // verdade
```

#### <= menor ou igual a
O operador menor ou igual retorna true (verdadeiro) se o operando da esquerda for menor ou igual ao operando da direita.

```javascript
3 <= 4 // verdade
```

### Operadores Lógicos

#### && E lógico 
Se o primeiro valor for verdadeiro, ou puder ser considerado ou convertido pra verdadeiro retorna o segundo valor.

Se o primeiro valor for falso, retorna falso.

```javascript
true && "oi" // "oi"
"oi" && true // true
true && false // false
```

#### || Ou lógico 
Se o primeiro valor for verdadeiro, ou puder ser considerado ou convertido pra verdadeiro retorna o primeiro valor.

Se o primeiro valor for falso, retorna o segundo valor.

```javascript
false || true // true
false || false // false
false || "oi" // "oi"
false || 0 // 0
```

#### ! Não lógico 
Esse operador inverte o valor de uma expressão

Obs: Se um valor pode ser convertido para verdadeiro, este valor é chamado de truthy. Se um valor pode ser convertido para falso, este valor é chamado de falsy.

Exemplos de expressões que podem ser convertidas para falso são:

- null;
- NaN;
- 0;
- string vazia (""); 
- undefined.

Todos os outros são considerados verdadeiros.

```javascript
!true // false
!false // true
!'Oi' // false
!'' // true
```

## Condicionais

Usamos para verificar uma condição e definir se algo deve ou não acontecer a partir da condição dada.

É a linguagem que utilizamos para nos comunicar, repare:

Se amanhã fizer sol, vou viajar para a praia.

Temos uma condição (Se amanhã fizer sol) para executar uma ação (viajar para a praia) dependendo do resultado dessa condição. Se verdadeira, a ação é executada.

### Expressões condicionais simples

```javascript
// Variável booleana verdadeira
var sol = true;

// Condição
if ( sol ) {
	// Ação
	alert('Vou viajar para a praia!');
}
```

### Estrutura if / else

```javascript
// Variável booleana verdadeira
var sol = false;

// Condição
if ( sol ) {
	// Ação
	alert('Vou viajar para a praia!');
}else{
	// Ação
	alert('Vou ao cinema');
}
```


### Estrutura if / else if / else

```javascript
// Variável booleana verdadeira
var hora = 8;

// Condição
if ( hora <= 12 ) {
	// Ação
	alert('Bom dia');
}else if( hora <= 18){
	// Ação
	alert('Boa tarde');
}else{
	// Ação
	alert('Boa noite');
}
```

```javascript
if ( condição ) {
	// Ação
} else if ( outra condição ) {
	// Ação
} else if ( outra condição ) {
	// Ação
} else if ( outra condição ) {
	// Ação
} else if ( quantas condições quiser ) {
	// Ação
} else {
	// Ação final se nenhuma condição for verdadeira
}
```

### Estrutura switch case
Se a condição for correspondida, o programa executa as instruções asssociadas. Se múltiplos casos corresponderem o valor, o primeiro caso que corresponder é selecionado, mesmo se os casos não forem iguais entre si.

```javascript
var dia = 'Segunda';

switch ( dia ) {
	case 'Segunda':
		alert('😴');
		break;
	case 'Terça':
		alert('😐');
		break;
	case 'Quarta':
		alert('🙂');
		break;
	case 'Quinta':
		alert('😬');
		break;
	case 'Sexta':
		alert('🤪');
		break;
	case 'Sábado':
		alert('😎');
		break;
	case 'Domingo':
		alert('😞');
		break;
	default:
		alert('Não achei sua condição.');
}
```

### Importância do break (switch case)
A instrução opcional break associada com cada case garante que o programa saia da condicional switch assim que a instrução correspondente for executada  e executa a instrução que segue logo após o switch. Caso break seja omitido, o programa continua a execução para a próxima instrução dentro de switch. 

Se você esquecer um break então o script irá rodar a partir do caso onde o critério foi correspondido e irá rodar também o caso seguinte independentemente do critério ter sido correspondido ou não:


```javascript
var dia = 'Segunda';

switch ( dia ) {
	case 'Segunda':
		alert('😴');
	case 'Terça':
		alert('😐');
	case 'Quarta':
		alert('🙂');
	case 'Quinta':
		alert('😬');
	case 'Sexta':
		alert('🤪');
	case 'Sábado':
		alert('😎');
	case 'Domingo':
		alert('😞');
	default:
		alert('Não achei sua condição.');
}
```

### Operador ternário
O operador condicional (ternário) é o único operador JavaScript que possui três operandos. Este operador é frequentemente usado como um atalho para a instrução if.

```javascript
var idade = 16;

var acesso = idade > 18 ? true : false;
```

A expressão antes do ? é a condição if, se for verdadeira o primeira ação é executada, caso contrário a segunda ação, a que vem depois dos :, é executada

É muito útil para testes mais básicos em que se tem apenas uma única linha de código dentro do if ou do else.

```javascript
var salario = 1000;
var bonus = salario * (salario > 1000 ? 0.10 : 0.15);
```

## Laços de repetição
Laços oferecem um jeito fácil e rápido de executar uma ação repetidas vezes. 

JavaScript suporta diferentes tipos de loops:

### for
Você pode pensar em um laço de repetição como um jogo onde você manda o seu personagem andar X passos.

```javascript
var passo;
for (passo = 1; passo <= 5; passo++) {
  // Executa 5 vezes, com os valores de passos de 1 a 5.
  console.log('já dei '+passo+' passos');
}
// já dei 1 passos
// já dei 2 passos
// já dei 3 passos
// já dei 4 passos
// já dei 5 passos
```

### for of
O JavaScript for/of instrução itera pelos valores de objetos iteráveis

for / of permite percorrer estruturas de dados que são iteráveis, como Arrays, Strings, Maps, NodeLists, and more.

```javascript
var txt = 'JavaScript';
var x;

for (x of txt) {
  console.log(x + "<br >");
}
```

## Funções e parâmetros

Uma função JavaScript é definida com a palavra-chave `function`, seguida por um **nome**(opcional), seguido por parênteses **()**.

Os nomes das funções podem conter letras, dígitos, sublinhados e cifrões (mesmas regras que as variáveis).

Os parênteses podem incluir nomes de parâmetros separados por vírgulas:
**(parâmetro1, parâmetro2, ...)**

O código a ser executado, pela função, é colocado entre colchetes: **{}**

```javascript
function nome(parametro1, parametro2, parametro3) {
  // código a ser executado
}
```

Os **parâmetros** da função estão listados entre parênteses () na definição da função.

Os **argumentos** da função são os **valores** recebidos pela função quando ela é chamada.

Dentro da função, os argumentos (os parâmetros) se comportam como **variáveis** locais.


## Arrays

Em Js o Array é um objeto, um objeto especial com características próprias mas não existe o nativo. Ele trabalha de uma forma indexada a partir de um valor inteiro começando com 0. É uma estrutura dinâmica que cresce dinamicamente e diminui dinamicamente diferente de outras linguagens na qual tem uma estrutura estática e tamanho fixo. Os tipos de dados que você pode colocar no Array são os mais variáveis possíveis ou seja, uma estrutura heterogênea em que você pode colocar um inteiro, um boolean, um objeto ou outro Array, não existe restrição. Dito isso a boa prática diz que você deve trabalhar com dados homogêneos dentro de um array.


### Acessando um item do array

```javascript
var arr = ['primeiro, 'segundo'];
console.log(arr[0]);// exibr 'primeiro'
console.log(arr[1]);// exibe 'segundo'
```
<!-- 
### Tamanho do array
A propriedade length retorna o número de elementos nessa matriz.

```javascript
var frutas = ['Fruta do Conde', 'Atemóia'];
console.log(frutas.length);
frutas[frutas.length - 1];
```

<img src="assets/length01.png">
<img src="assets/length02.png">

### Adicionando um item no array

#### final do Array
```javascript
frutas.push('Laranja');
// ['Fruta do Conde', 'Atemóia', 'Laranja'];
```

#### começo do Array
```javascript
frutas.unshift('Morango');
// ['Morango','Fruta do Conde', 'Atemóia', 'Laranja'];
```

### Removendo um item do array

#### final do Array
```javascript
frutas.pop(); // remove Laranja (do final)
// ['Morango','Fruta do Conde', 'Atemóia', 'Laranja'];
```

#### início do Array

```javascript
frutas.shift(); // remove Morango do início
// ['Fruta do Conde', 'Atemóia', 'Laranja'];
```
#### Procurar o índice de um item

```javascript
var pos = frutas.indexOf('Atemóia');
```

### Remover item por indice

```javascript
var removedItem = frutas.splice(pos, 1);
//recorta um item de um array
// ['Fruta do Conde', 'Laranja'];
```

#### Remover itens

```javascript
var vegetais = ['Repolho', 'Nabo', 'Rabanete', 'Cenoura'];
var pos = 1, n = 2;
var itensRemovidos = vegetais.splice(pos, n); 
// a partir da posição (pos) em direção ao fim da array.

console.log(vegetais); 
// ['Repolho', 'Cenoura'] (o array original é alterado)
console.log(itensRemovidos); 
// ['Nabo', 'Rabanete']
```

#### Copiar um Array

```javascript
var copiar = frutas.slice(); 
// ['Morango', 'Manga']

var copiar = frutas.slice(posicao, posicao+1); // ['Morango', 'Manga']
```


### 🌵Foreach

```javascript
const aprovados = ['Agatha', 'Aldo', 'Daniel', 'Raquel']
aprovados.forEach(function(nome, indice, array){
    console.log(`${indice + 1}) ${nome}`)
    console.log(array)
})

aprovados.forEach(nome => console.log(nome))


const exibirAprovados = aprovado => console.log(aprovado)
aprovados.forEach(exibirAprovados)
```

### 🌵Map
O método `map()` mapeia o array para o outro array do mesmo tamanho só que com os dados transformados

```javascript
const nums = [1,2,3,4,5]

let resultado = nums.map(function(e){
    return e * 2
})

console.log(resultado) // [ 2, 4, 6, 8, 10 ]

const soma10 = e => e + 10 
const triplo = e => e * 3
const paraDinheiro = e => `RS ${parseFloat(e).toFixed(2).replace(".",",")}`


console.log(nums.map(soma10).map(triplo).map(paraDinheiro)) //[ 'RS 33,00', 'RS 36,00', 'RS 39,00', 'RS 42,00', 'RS 45,00' ]

// outro exemplo

const carrinho = [
    '{ "nome": "Borracha", "preco": 3.45 }',
    '{ "nome": "Carderno", "preco": 13.90 }',
    '{ "nome": "Kit de Lapis", "preco": 41.22 }',
    '{ "nome": "Caneta", "preco": 7.50 }',
]

const obj = json => JSON.parse(json)
const showPrice = produto => produto.preco

const result =  carrinho.map(obj).map(showPrice)
console.log(result) // [ 3.45, 13.9, 41.22, 7.5 ]
```

#### Filter
O método `filter()` cria um novo array com todos os elementos que passaram no teste implementado pela função fornecida.

```javascript
const produtos = [
    { "nome": "Notebook", "preco": 2445, fragil: true },
    { "nome": "Ipad", "preco": 4199, fragil: true },
    { "nome": "Copo de Vidro", "preco": 12.22, fragil: true },
    { "nome": "Copo de Plástico", "preco": 18.22, fragil: false },
]

console.log(produtos.filter(function(p){
    return false
})) // []

const caro = produto => produto.preco >= 500
const fragil = produto => produto.fragil

console.log(produtos.filter(caro).filter(fragil)) // [ { nome: 'Notebook', preco: 2445, fragil: true }, { nome: 'Ipad', preco: 4199, fragil: true } ]
```

#### Reduce
O método `reduce()` serve para transformar um array, reduzindo-o ou agregando-o os valores um só, podendo ser esse elemento um array, um número, string, etc

```javascript
const alunos = [
    { "nome": "João", "nota": 7.6, bolsista: false },
    { "nome": "Maria", "nota": 9.8, bolsista: true },
    { "nome": "Pedro", "nota": 9.3, bolsista: false },
    { "nome": "Ana", "nota": 8.7, bolsista: true }
]

const resultado = alunos.map( a => a.nota).reduce(function(acumulador, atual){
    console.log(acumulador, atual)
    return acumulador + atual
}, 0) //valor inicial

console.log(resultado) 
// 0 7.6
// 7.6 9.8
// 17.4 9.3
// 26.7 8.7
// 35.4

//1: todos os bolsistas
const todosBolsistas = (resultado, bolsista) => resultado && bolsista
console.log(alunos.map( a => a.bolsista).reduce(todosBolsistas)) // false

//2: algum aluno é bolsista

const isBolsista = (resultado, bolsista) => resultado || bolsista
console.log(alunos.map( a => a.bolsista).reduce(isBolsista)) // true

```

#### Concat

```javascript
const filhas = ['Julia','Paula']
const filhos = ['Pedro','João']
const todos = filhas.concat(filhos)
console.log(todos) // [ 'Julia', 'Paula', 'Pedro', 'João' ]

```

#### Operador Rest/Spread

```javascript
//operador ... rest(juntar)/spread(espalhar)
//usar rest com parâmetro de função

//usar spread com array
const grupoA = = [ 'João', 'Pedro', 'Glória']
const grupoFinal = [ 'Maria', ...grupoA, 'Rafaela']
console.log(grupoFinal) // [ 'Maria', 'João', 'Pedro', 'Glória', 'Rafaela' ]
``` -->