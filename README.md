# imperativaIDH
parcial 1



const prompt = require("prompt-sync")({ sigint: true });

/** Ejercicio #1: 
Realizar una función que reciba por parámetro dos valores numéricos. 
Si ambos números recibidos son impares se deberá retornar su división. 
En cambio, si ambos números recibidos son pares entonces se deberá retornar la suma. 
Para cualquier otro caso, retornar  null **/

const ejericico01 = (num01,num02) => {
    if(num01 % 2 !== 0 && num02 % 2 !== 0){
        return num01 / num02;
    }

    else if(num01 % 2 === 0 && num02 % 2 === 0){
        return num01 + num02;
    }

    else{
        return null;
    }
}

console.log('Digite dos numeros: ');

let num01 = prompt();
let num02 = prompt();

console.log(ejericico01(num01,num02));


/* Ejercicio #2:
Desarrollar una función que reciba un array de notas (representado por 4 numeros 
enteros positivos) [7,6,7,8] por parámetro, calcule él promedio y retorne:
    - retornar true SI  él promedio es mayor a 7
    - caso contrario retornar false 

let notas = [9,7,7,9]

function obtenerPromedio (arrayNotas){
    let suma = 0;
    for (let index = 0; index < arrayNotas.length; index++) {
        suma = suma + arrayNotas[index];
    }

    let promedio = suma / arrayNotas.length;
    if(promedio > 7){
        return true;
    }
    else{
        return false;
    }
}


console.log(obtenerPromedio(notas));

**/

/* -Ejercicio #3:
Dado el siguiente array de objetos literales que representan artículos
Realizar una función que reciba por parámetro el array de artículos, y  un valor 
numérico que represente al precio máximo , deberá retornar un nuevo array con los 
artículos que cumplan con estas condiciones.

let articulos = [
    {
        id: 4 ,
        precio : 3321,
        tipo : "Deportivo",
        nombre: "Zapatillas"
    },

    {
        id: 22 ,
        precio: 4482,
        tipo : "Moda",
        nombre: "Zapatillas"
    },

    {
        id: 1 ,
        precio: 3600,
        tipo : "Moda",
        nombre: "Zapatos"
    },

    {
        id: 44 ,
        precio: 8889,
        tipo : "Moda",
        nombre: "Remera"
    },
]

const ejercicio03 = (arrayArticulos,valorNum) => {
    let newArray = []
    for (let i = 0; i < arrayArticulos.length; i++) {
       if (arrayArticulos[i].precio < valorNum) {
            newArray.push(arrayArticulos[i]);
       }
    }
    return newArray;
}

console.table(ejercicio03(articulos,4000));
*/
