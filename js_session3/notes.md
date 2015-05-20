Recorriendo un arreglo con while

var names = ["Juan","Pedro","Oscar"];
var counter = 0;

while (counter < names.length){
 console.log(names[counter]);
    counter++;
}

=====================================
Recorriendo un arreglo con for

var names = ["Juan","Pedro","Oscar"];
var counter = 0;

for( i = 0; i < names.length; i++){
    console.log(names[i]);  
}

============================================
var firstNames = ["Juan", "Pedro"];
var lastNames = ["Henández", "Ramírez"];

firstNames.shift();
console.log(firstNames);

firstNames.unshift("Ramiro");
console.log(firstNames);

firstNames.sort(lastNames);
console.log(firstNames);

firstNames.concat(lastNames);
console.log(firstNames);

firstNames.join(", ");
console.log(firstNames);

====================================
.map

var firstNames = ["Juan", "Pedro"];
var lastNames = ["Henández", "Ramírez"];

var fullNames = firstNames.map(function(firstName){ return firstName + " Perez"});
console.log(fullNames);

=======================================
.reduce

var numbers = [ 1, 2, 3, 4, 5];

numbers.reduce(function(prevValue, currValue, index, array){
 return prevValue + currValue;   
});

=====================================
filtering

var ages = [10, 15, 16, 17, 18, 20, 33, 54];

var grownUps = ages.filter(function(age) {
                           return age >= 18;
                           });
console.log(grownUps);

===================================
hashes / Diccionarios , objetos literales

var people = [
    {    name : "Oscar",
     age: 24,
     petName : ["Perro", "Cocodrilo"]
    },
    {
        name : "Iván",
        age :14,
        petName : ["Gato","Gato2"]
    },
    {
        name: "Juan",
        age : 67,
        petName :[]
    }
        ];

var noPet = people.filter(function(person){
return person.petName.length ==0;
}).map(function(person){
   return person.name; 
});
    

console.log(noPet);

================================
URL: ufe9o17v
===============================
Ejercicio integrador:

var people = [{name: "Oscar", age: 21, gender: "Male"}, 
              {name: "Rocío", age: 15, gender: "Female"},
              {name: "Iván", age: 15, gender: "Male"},
              {name: "Sandra", age: 15, gender: "Female"},
              {name: "Mari", age: 67, gender: "Female"}];

function freeAdmition(person){}
function outPut(){}
function entranGrtis(people){
    var free = people.filter(function(person)){
                 
                 return freeAdmition(person);
                 });

outPut(free);

}
==================================================
Tarea terminar piedra, papel y tijeras con functions

    
    function isTied(player1, player2){
        return player1 == player2;   
    }
    function rockWin(player1, player2){
        var array = [player1, player2];
        return arrayIncludes(array, "Tijeras") && arrayIncludes(array, "Piedra");
    }
    
    function paperWin(player1, player2){
        var array = [player1, player2];
        return arrayIncludes(array, "Papel") && arrayIncludes(array, "Piedra");
        
    }
    
    function scissorsWin(player1, player2){
        var array = [player1, player2];
        return arrayIncludes(array, "Tijeras") && arrayIncludes(array, "Papel");
        
    }
