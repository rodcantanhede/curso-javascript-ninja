# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function primeira (x, y) { 
return x + y;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var recebedora = primeira(5, 5) + 5;

// Qual o valor atualizado dessa variável?
15

// Declare uma nova variável, sem valor.
var semval;


// Crie uma função que adicione um valor à variável criada acima, e retorne a string:

function segunda () {
semval = 10;
return "O valor da variável agora é " + semval;

// Invoque a função criada acima.
segunda()

// Qual o retorno da função? (Use comentários de bloco).
/*O valor da variável agora é 10 */

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function terceira (x, y, z) {
if( x == "" || y == "" || y == "") {
return "Preencha todos os valores corretamente!";
}
return (x * y * z) + 2;
}

// Invoque a função criada acima, passando só dois números como argumento.
terceira(2, 4);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
//Preencha todos os valores corretamente!

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
terceira(2, 4, 6);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
//50

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/

function quarta(x, y, z) {
if(x != "" && y == "" && z == "") { 
return x;
} else if ( y != "" && x == "" && z == "") {
return y; 
} else if (z != "" && y == "" && x == "") {
return z;
} else if (x != "" && y != "" && z == "") {
return x + y;
} else if (x != "" && y == "" && z != "") {
return x + z;
} else if (x == "" && y != "" && z != "") {
return y + z;
} else if( x != "" && y != "" && z != "") {
return (x + y) / z;
} else if (x == "" || y == "" || z == "") {
return false;
} else { 
return null;
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
?
quarta ();
quarta (2);
quarta (2, 4);
quarta (2, 4, 6);
