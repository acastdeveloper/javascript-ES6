| Objectius | Practicar ES6: literals, funcions fletxa, .map(), forEach(), spread operator...                                                                 |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Entrega   | - Pujar la URL del repositori anomenat javascript-ES6 que contingui la solució al campus virtual.<br>- Cada exercici en un commit diferent.<br> |
| Temps     | 4-6 dies                                                                                                                                        |
| Recursos  | https://scrimba.com/g/gintrotoes6                                                                                                               |

## <u>Nivell I</u>

Aquest exercici és molt senzill: **es plantegen petits fragments de codi JavaScript ES5, els quals s'han de reescriure per a utilitzar la nomenclatura d'ES6 i resoldre petits reptes mitjançant ES6.**

<mark>L'objectiu és repassar els coneixements adquirits d'ES6.</mark>

### Exercici 1

Converteix a funcions fletxa:

```js
function multiply(num1, num2) {
     return num1 * num2;
}

function toCelsius(fahrenheit) {
     return (5/9) * (fahrenheit-32);
}

// This function returns a string padded with leading zeros
function padZeros(num, totalLen) {
    var numStr = num.toString();
    var numZeros = totalLen - numStr.length;

    for (var i = 1; i <= numZeros; i++) {
        numStr="0" + numStr;
    } 

    return numStr;
 } 

function power(base, exponent) {  
     var result=1; 
     for (var i=0; i < exponent; i++) { 
         result *=base; 
     } 

 return result;
} 

function greet(who) {
 console.log("Hello " + who);
}
```

### Exercici 2

Arregla l'error del següent bloc de codi:

```js
users.map(function (user) {
 user.firstName;
});

var users = 
[{ firstName: 'Homer', lastName: 'Simpson' },
{ firstName: 'Marge', lastName: 'Simpson' },
{ firstName: 'Bart', lastName: 'Simpson' },
{ firstName: 'Lisa', lastName: 'Simpson' },
{ firstName: 'Maggie', lastName: 'Simpson' }];
```

### Exercici 3

Donat el següent array de strings, mostrar per consola la frase completa usant .reduce()

```js
var epic = ['a', 'long', 'time', 'ago', 'in a', 'galaxy', 'far far', 'away'];
```

Resultat per consola: 'a long time ago in a galaxy far far away'

**Nota**: no fa falta fer un "join".

### Exercici 4

Crear una funció que accepti un string i retornada aquest string revertit. Nota: Usar funció fletxa (arrow functions), l'operador de prograpación (spread operator) y el *mètode .reverse()*

### Exercici 5

Modifica la funció 'a()' per a reemplaçar la promesa per aync/await:

```js
function b() {
 // tasques asíncrones , que triguen una estona..

}

funtion a() {
 // Ens esperem que la funció b acabi

 b().then() = > {
 doMoreWork();
 }

}
```

### Exercici 6

Tenim un array de tasques i volem aconseguir un array que contingui únicament els noms de les tasques. 

- Usar .forEach() per obtenir aquest array.

- Usar .map() per obtenir aquest array.

```js
var tasks = [

{
 'name' : 'Start React web',
 'duration' : 120
},

{
 'name' : 'Work out',
 'duration' : 60
},

{
 'name' : 'Procrastinate on facebook',
 'duration' : 240
}

];
```

## <u>Nivell II</u>

### Exercici 7

Realitzar un programa en ES6, amb al menys una funció.

Aquest programa demana a l'usuari dos nombres de l'1 a l'10 (con [promp](https://www.w3schools.com/jsref/met_win_prompt.asp) es suficient). 

Un cop introduïts, es mostra per consola la taula de multiplicar del número 1 que va fins al número 2.

Per exemple, si l'usuari introdueix 3 i 5:

3 X 1 = 3
3 X 2 = 6
3 X 3 = 9
3 X 4 = 12
3 X 5 = 15

### Exercici 8

Modificar l'exercici anterior perquè els números s'introdueixin a través d'un formulari (amb validacions), i que la taula de multiplicar la mostri en una taula HTML.

## <u>Nivell III</u>

### Exercici 9

Aquest exercici tracta de crear un cercador. Donada una llista de noms, a l'introduir un nom al cercador només s'han de mostrar aquells que coincideixin.

Seria desitjable que vagi filtrant conforme es va omplint el nom. També tenir en compte maquetar la solució final perquè tingui bon aspecte. 



Code snippet:

```html
<ul id="myUL">
  <li><a href="#">Albert</a></li>
  <li><a href="#">Ismael</a></li>
  <li><a href="#">Luis</a></li>
  <li><a href="#">Rubén</a></li>
  <li><a href="#">Jonatan</a></li>
  <li><a href="#">Jake</a></li>
  <li><a href="#">Jose</a></li>
</ul>
```
