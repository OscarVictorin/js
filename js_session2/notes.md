Ejemplo: do while (adivina contraseña)


var password = "password";
var usserPassword = "";

do{
    userPassword = prompt("Dime el password");
    
} while(userPassword != password);

alert("Estás logueado");
==================================================
Ejemplo: while (adivina contraseña)

var password = "password";
var userPassword = "";

while(userPassword != password) {
    userpassword = prompt("Ingresa tu password: ");   
};

alert("Bienvenido");

===================================================
Ejemplo: pregunta secreta más password:
var password = "password";
var userPassword = "";
var userQuestion = "respuesta";
var userAnswer = "";

while(userPassword != password) {
    while(userAnswer != userQuestion){
        
        userAnswer = prompt("Respuesta a pregunta secreta: ");   
};
    userPassword = prompt("Introduce tu contraseña: ");

}

alert("Bienvenido");

==============================================
Ejemplo: Limitar intentos password

var password = "password";
var userPassword = "";
for(var i = 0; i < 10; i++){
 userPassword = prompt("Cuál es tu password?" );
    if (userPassword == password)
    {
        alert("Bienvenido");
        break;
    }
    else
    {
        alert("Inténtalo de nuevo");
    }
}
===========================================
Ejemplo: Sumando todos los números

var upTo = prompt("Hasta qué número quieres sumar?");
var sum = 0;

for(var i = 1; i <= upTo; i++){
     sum = sum + i;  
}
alert(sum);

============================================
Ejemplo: Calcular śi un número es primo

var number = parseInt(prompt("Digita un número"));
var primo = true;

if (number <= 1) 
    {
        primo = false;
    alert("No es primo");
    }

else {
for (var i = 2; i < number; i++)
    {
        if (number % i == 0) 
        {
            primo = false;
        alert("No es un número primo");
            break;
        }
    }
}
if(primo)
{alert("Es primo!!!!!");
}
==========================================
Tarea= Generar número primos 



==========================================
Arreglos:

var userList = ["Juan", "Pedro", 10, 10.50];
var emptyList = [];

for(var i = 0; i < userList.length; i++){
    console.log(userList[i]);   
}