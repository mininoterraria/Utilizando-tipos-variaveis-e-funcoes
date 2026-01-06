01. Declare três variáveis diferentes (uma para cada tipo: string, número e booleano) e atribua valores a elas. Em seguida, exiba o tipo de cada variável no console.
```js
const string = 'Diego';
const numero = 21;
const booleano = true;

console.log(typeof(string));
console.log(typeof(numero));
console.log(typeof(booleano));
```
02. Crie duas variáveis, uma contendo seu primeiro nome e outra contendo seu último nome. Em seguida, combine-as em uma terceira variável usando o operador + e em uma quarta variável usando template strings. Por fim, imprima os resultados obtidos no console.
```js
const nome = 'Diego';
const ultimoNome = 'Araújo';
const combinacao1 = nome + ' ' + ultimoNome;
const combinacao2 = `\n${nome} ${ultimoNome}`
console.log(combinacao1, combinacao2);
```
03. Declare duas variáveis, uma contendo um número e outra contendo uma string. Em seguida, combine-as em uma terceira variável usando template strings para montar uma frase e exiba o resultado no console.
```js
const numero = 21;
const string = 'Sua idade é:';
const combinacao = `${string} ${numero} anos`;
console.log(combinacao);
```
04. Crie uma variável inicializada com um valor de qualquer tipo e, em seguida, reatribua um novo valor a essa variável. Imprima ambos os valores no console após atribuí-los.
```js
let variavel;
console.log(variavel);
variavel = 'feijão';
console.log(variavel);
```
05. Declare uma variável usando var fora de um bloco de código (por exemplo, if) e outra dentro desse bloco. Tente acessar essas variáveis dentro do bloco e fora dele utilizando console.log e analise os resultados. Faça o mesmo processo utilizando let e compare com os resultados anteriores.
```js
let booleano1 = true;
console.log(booleano1);

if(true){ 
    let booleano1 = false;
    console.log(booleano1);
}

console.log(booleano1);

console.log(`\n`);

var booleano2 = true;
console.log(booleano2);

if(true){
    var booleano2 = false;
    console.log(booleano2);
}

console.log(booleano2);
    //Resultado: Com var, a variável de mesmo nome pode ser alterada tanto dentro quanto fora do escopo global, com let, cada uma das variáveis são independentes, com valores únicos ao seu escopo.
```
06. Declare uma variável booleana que informa se está chovendo e utilize-a em uma estrutura condicional (if) para exibir uma mensagem informando se é preciso levar um guarda-chuva ou não dependendo do valor da variável.
```js
const booleano = true;

if(booleano){
    console.log("Precisa levar um guarda-chuva.");
}else{
    console.log("Não precisa levar um guarda-chuva.");
}
```
07. Crie uma variável contendo uma frase. Em seguida, exiba no console o comprimento da frase e a mesma frase com letras maiúsculas.
```js
const frase = 'Olá meu povo tudo bom?';
console.log(`Comprimento da frase: ${frase.length} \nFrase: ${frase.toUpperCase()}`);
```
08. Declare duas variáveis, uma inicializada com valor null e outra que não recebe atribuição (resultando em undefined). Exiba os valores no console.
```js
let variavel1 = null;
let variavel2;

console.log(variavel1);
console.log(variavel2);
```
09. Crie 3 variáveis de tipos diferentes, utilize template strings para combinar os diferentes tipos de dados (number, string, boolean) em uma única string e exiba o resultado no console.
```js
const variavel1 = 25;
const variavel2 = 'Olá!';
const variavel3 = true;
const stringResultado = `${variavel1}, ${variavel2}, ${variavel3}`;
console.log(stringResultado);
```
10. Crie uma variável numérica e uma string. Faça a conversão da variável numérica para string e da string para número. Exiba os tipos de dados resultantes no console.
```js
let numero = 5;
let string = '2';

console.log(numero);
console.log(string);
console.log('\n');

numero = String(numero);
string = Number(string);

console.log(numero);
console.log(string);
```
11. Crie uma variável com uma string e utilize métodos de manipulação de strings, como toUpperCase, toLowerCase, slice ou outros, para modificar a string original. Exiba os resultados finais no console.
```js
let string = 'Feijão é muito bom!';
console.log(string.toUpperCase());
console.log(string.toLowerCase());
console.log(string.slice(0,6));
```
12. Crie variáveis que armazenem o valor do saldo, de depósito e de um saque de uma conta bancária, depois realize operações de adição e subtração entre eles utilizando uma variável chamada operacao, considerando a função de cada variável criada anteriormente. Exiba os resultados finais no console.
```js
let saldo = 1000;
let deposito = 200;
let saque = 100;

const operacaoSaque = saldo -= saque;
const operacaoDeposito = saldo += deposito;

console.log(operacaoSaque);
console.log(operacaoDeposito);
```
13. Crie uma variável numérica com um valor. Utilize um operador ternário para verificar se esse valor é par ou ímpar. Exiba o resultado no console.
```js
const numero = 2;
numero % 2 === 0 ? console.log('Esse número é par!') : console.log("Esse número é impar!");
```
14. Considere uma situação em que você está verificando se um usuário está logado e tem permissão de administrador para acessar determinada funcionalidade. Utilize variáveis booleanas para simular essas condições e use o operador AND para verificar se ambas são verdadeiras.
```js
const login = false;
const contaAdministrador = true;

if(login && contaAdministrador){
    console.log("Logado com sucesso!");
}else{
    console.log("Erro ao tentar logar!");
}
```
15. Declare duas variáveis booleanas e use o operador OR para verificar se pelo menos uma delas é verdadeira. Exiba o resultado no console
```js
const booleano1 = true;
const booleano2 = false;

if(booleano1 || booleano2){
    console.log("Uma das variáveis é verdadeira!");
}else{
    console.log("Nenhuma das variáveis é verdadeira!");
}
```
16. Imagine um sistema que determina se um usuário tem idade suficiente para comprar o ingresso para um show. Declare duas variáveis que determinem a idade mínima e qual a idade do usuário e utilize estruturas condicionais (if, else) para determinar se o usuário pode realizar a compra.
```js
const idadeMinima = 18;
const idadeUsuario = 20;

if(idadeUsuario >= idadeMinima){
    console.log("Pode comprar de boa!");
}else{
    console.log("Não pode comprar!");
}
```
17. Crie uma função que receba o nome de uma pessoa como argumento e retorne uma saudação personalizada. Em seguida, chame a função e exiba a saudação no console.
```js
const saudarAmigo = (nome) => `Olá, ${nome}!`;

console.log(saudarAmigo('arroz'));
```
18. Crie uma função que receba a idade de uma pessoa e retorne se ela é maior de idade (idade >= 18). Imprima o resultado no console.

```js
const validarIdade = (idade) => {
    if(idade >= 18){
        return 'É maior de idade!';
    }else{
        return 'É menor de idade!';
    }
}

console.log(validarIdade(18));
```
19. Crie uma função que receba uma string e verifique se é um palíndromo (uma palavra que é lida da mesma forma de trás para frente) utilizando o método de string reverse(). Retorne true se for um palíndromo e false caso contrário. Imprima o resultado no console.
```js
const verificarPalindromo = (string) => {
    const reverterString = string.split('').reverse().join('');

    if(reverterString === string){
        return true;
    }else{
        return false;
    }
}

console.log(verificarPalindromo('ara'));
```
20. Crie uma função que receba três números como parâmetros e determine qual é o maior entre eles. Utilize estruturas condicionais (if, else) para comparar os valores e determinar o maior. Imprima o maior valor no console.
```js
const maiorNumero = (a,b,c) => {
    if(a > b && a > c){
        return a;
    }else if (b > a && b > c){
        return b;
    }else if(c > a && c > b){
        return c;
    }
}

const resultado = maiorNumero(4,2,3);

console.log(`O maior número é: ${resultado}`);
```
21. Crie uma arrow function chamada calculaPotencia que receba dois parâmetros: a base e o expoente. A função deve calcular a potência da base elevada ao expoente e retornar o resultado.
```js
const calculaPotencia = (base, expoente) =>  base ** expoente;

console.log(calculaPotencia(3,4));
```
