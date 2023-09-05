# Exemplos de `Métodos de Arrays` JavaScript

Neste arquivo, apresentamos exemplos de vários métodos JavaScript úteis para lidar com arrays.

## Método 1: `length`

O método `length` retorna o número de elementos em um array.

**Exemplo:**
```javascript
const frutas = ['maçã', 'banana', 'pera'];
const quantidadeDeFrutas = frutas.length;
console.log(quantidadeDeFrutas); // Output: 3
```

## Método 2: `push`

O método `push()` adiciona um ou mais elementos ao final de um array e retorna o novo comprimento do array.

**Exemplo:**
```javascript
frutas.push('laranja');
console.log(frutas); // Output: ['maçã', 'banana', 'pera', 'laranja']
```

## Método 3: `pop`

O método `pop()` remove o último elemento de um array e retorna esse elemento removido.

**Exemplo:**
```javascript
const ultimoElemento = frutas.pop();
console.log(ultimoElemento); // Output: 'laranja'
```

## Método 4: `unshift`

O método `unshift()` adiciona um ou mais elementos ao início de um array e retorna o novo comprimento do array.

**Exemplo:**
```javascript
frutas.unshift('morango');
console.log(frutas); // Output: ['morango', 'maçã', 'banana', 'pera']
```

## Método 5: `shift`

O método `shift()` remove o primeiro elemento de um array e retorna esse elemento removido.

**Exemplo:**
```javascript
const primeiroElemento = frutas.shift();
console.log(primeiroElemento); // Output: 'morango'
```

## Método 6: `includes`

O método `includes()` verifica se um elemento está presente em um array e retorna `true` ou `false`.

**Exemplo:**
```javascript
const contemPera = frutas.includes('pera');
console.log(contemPera); // Output: true
```

## Método 7: `reverse`

O método `reverse()` inverte a ordem dos elementos em um array.

**Exemplo:**
```javascript
frutas.reverse();
console.log(frutas); // Output: ['pera', 'banana', 'maçã']
```

## Método 8: `join`

O método `join()` cria uma string a partir dos elementos de um array, usando um separador especificado.

**Exemplo:**
```javascript
const frase = frutas.join(', ');
console.log(frase); // Output: 'pera, banana, maçã'
```

## Método 9: `concat`

O método `concat()` combina dois ou mais arrays em um novo array.

**Exemplo:**
```javascript
const frutas2 = ['uva', 'abacaxi'];
const todasAsFrutas = frutas.concat(frutas2);
console.log(todasAsFrutas); // Output: ['pera', 'banana', 'maçã', 'uva', 'abacaxi']
```

## Método 10: `slice`

O método `slice()` cria uma cópia superficial de parte de um array e a retorna como um novo array.

**Exemplo:**
```javascript
const copia = todasAsFrutas.slice(1, 4); // Cria uma cópia dos elementos 1 a 3 (não incluindo o 4)
console.log(copia); // Output: ['banana', 'maçã', 'uva']
```

## Método 11: `splice`

O método `splice()` adiciona, remove ou substitui elementos em um array.

**Exemplo:**
```javascript
const numeros = [1, 2, 3, 4, 5];
numeros.splice(2, 1); // Remove o elemento de índice 2
console.log(numeros); // Output: [1, 2, 4, 5]
```

## Método 12: `every`

O método `every()` verifica se todos os elementos de um array atendem a uma condição.

**Exemplo:**
```javascript
const todosSaoMaioresQueZero = numeros.every(numero => numero > 0);
console.log(todosSaoMaioresQueZero); // Output: true
```

## Método 13: `some`

O método `some()` verifica se pelo menos um elemento de um array atende a uma condição.

**Exemplo:**
```javascript
const algumEhMaiorQueCinco = numeros.some(numero => numero > 5);
console.log(algumEhMaiorQueCinco); // Output: false
```

## Método 14: `find`

O método `find()` retorna o primeiro elemento de um array que atende a uma condição.

**Exemplo:**
```javascript
const primeiroMaiorQueTres = numeros.find(numero => numero > 3);
console.log(primeiroMaiorQueTres); // Output: 4
```

## Método 15: `map`

O método `map()` cria um novo array com base em uma transformação aplicada a cada elemento do array original.

**Exemplo:**
```javascript
const aoQuadrado = numeros.map(numero => numero ** 2);
console.log(aoQuadrado); // Output: [1, 4, 9, 16, 25]
```

## Método 16: `filter`

O método `filter()` cria um novo array com todos os elementos que atendem a uma condição.

**Exemplo:**
```javascript
const maioresQueDois = numeros.filter(numero => numero > 2);
console.log(maioresQueDois); // Output: [3, 4, 5]
```

## Método 17: `sort`

O método `sort()` classifica os elementos de um array em ordem alfabética ou numérica.

**Exemplo:**
```javascript
const nomes = ['Ana', 'Carlos', 'Eva', 'David'];
nomes.sort();
console.log(nomes); // Output: ['Ana', 'Carlos', 'David', 'Eva']
```

## Método 18: `reduce`

O método `reduce()` executa uma função em cada elemento do array, acumulando um resultado.

**Exemplo:**
```javascript
const soma = numeros.reduce((acumulador, numero) => acumulador + numero, 0);
console.log(soma); // Output: 15
``