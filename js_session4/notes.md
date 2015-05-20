Session 4

Funciones

var trueAndFalse = function (a, b){
    return a === b;
}

console.log(trueAndFalse(5, 5));
========================================
Variables globales

var firstName ="Adela";
var age = 65;
var person = {name: "Pedro", age: 60};

var myFunc = function(){
    firstName = "Juan";
}

{
    var agePlusOne = function(person){
     person.age = person.age + 1;   
    }
}

console.log(firstName);
myFunc();
console.log(firstName);
agePlusOne(person);
console.log(person.age);

=======================================
function hello(outPutter){
 outPutter("Hola mundo");   
}

function consoleOutput(myString){
 console.log(myString);   
}

hello(consoleOutput);

======================================
function sum10(){
 var acum = 0;
    return function(){
     acum = acum + 10;
        return acum;
    }
}

var plus10 = sum10();
console.log(plus10());
console.log(plus10());
console.log(plus10());
console.log(plus10());

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