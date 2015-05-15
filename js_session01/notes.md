var isVerified = true;
console.log(isVerified);

var addres = "Monterrey NL";
console.log(addres);

var age = 19;
console.log(age);

var price = 0.99;
console.log(price);

var name;
console.log(name)

var nullValue = null;
console.log(nullValue)

======================================

var speed = 10.10;
var age = 10;
var firstName = "Oscar"

console.log(speed > 11 && age < 11);
console.log(speed > 9 || age <12);
console.log(speed !== age);

========================================

var isMale = true;
var age = 20;
var email = "oscar@latam.com";
var nullValue = null;
var date;

console.log(typeof isMale);
console.log(typeof age);
console.log(typeof email);
console.log(typeof nullValue);
console.log(typeof date);

=======================================
var age = prompt("Digita tu edad");
var gender = "female";
var isMom = true;

if(isMom){
    alert("Feliz 10 de mayo");
}

if (age >= 18 && gender == "female"){
    alert ("Entra gratis!!");
    
} else {
    alert("Págale");
}
========================================
var player1 = prompt("Player 1: Piedra, papel o tijera?")
var player2 = prompt("Player 2: Piedra, papel o tijera?")

if(player1 === player2){
    alert("Empate");
}
else if(player1 == "piedra" && player2 == "tijera"){
 alert("Ganador player1");   
}
else if(player1 == "piedra" && player2 == "papel"){
 alert("Ganador player2");   
}
else if(player1 == "papel" && player2 == "piedra"){
 alert("Ganador player1");   
}
else if(player1 == "papel" && player2 == "tijera"){
 alert("Ganador player2");   
}