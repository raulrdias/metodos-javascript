# Exemplos de `Métodos de Strings` JavaScript

Neste arquivo, apresentamos exemplos de vários métodos JavaScript úteis para lidar com strings.

## Método 1: `includes()`

"O método `includes()` verifica se uma substring está presente em uma string e retorna `true` ou `false`."

**Exemplo:**
```javascript
const texto = 'Olá, mundo!';
const contemOla = texto.includes('Olá');
console.log(contemOla); // Output: true
```
## Método 2: `indexOf()`

"O método `indexOf()` retorna o índice da primeira ocorrência de uma substring em uma string, ou -1 se a substring não for encontrada."

**Exemplo:**
```javascript
const texto = 'Olá, mundo!';
const indiceOla = texto.indexOf('l');
console.log(indiceOla); // Output: 1
```

## Método 3: `slice()`

"O método `slice()` cria uma cópia superficial de parte de uma string e a retorna como uma nova string."

**Exemplo:**
```javascript
const texto = 'Isso é uma string de exemplo';
const novaString = texto.slice(5, 13); // Pega os caracteres do índice 5 (inclusive) ao 13 (exclusive)
console.log(novaString); // Output: 'é uma st'
```

## Método 4: `replace()`

O método `replace()` substitui a primeira ocorrência de uma substring por outra substring em uma string.

**Exemplo:**
```javascript
const texto = 'Olá, mundo!';
const novoTexto = texto.replace('mundo', 'todos');
console.log(novoTexto); // Output: 'Olá, todos!'
```

## Método 5: `toUpperCase()`

O método `toUpperCase()` converte todos os caracteres de uma string em maiúsculas.

**Exemplo:**
```javascript
const palavra = 'JavaScript';
const maiusculas = palavra.toUpperCase();
console.log(maiusculas); // Output: 'JAVASCRIPT'
```

## Método 6: `trim()`

O método `trim()` remove espaços em branco no início e no final de uma string.

**Exemplo:**
```javascript
const textoComEspacos = '   Olá, mundo!   ';
const textoSemEspacos = textoComEspacos.trim();
console.log(textoSemEspacos); // Output: 'Olá, mundo!'
```

## Método 7: `padStart()`

O método `padStart()` preenche o início de uma string com caracteres até atingir um comprimento especificado.

**Exemplo:**
```javascript
const numero = '42';
const numeroFormatado = numero.padStart(5, '0'); // Preenche com '0' até ter 5 caracteres
console.log(numeroFormatado); // Output: '00042'
```

## Método 8: `split()`

O método `split()` divide uma string em um array de substrings com base em um delimitador especificado.

**Exemplo:**
```javascript
const frase = 'Olá, como vai?';
const palavras = frase.split(' ');
console.log(palavras); // Output: ['Olá,', 'como', 'vai?']
```