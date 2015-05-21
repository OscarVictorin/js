var person = {
    fullName: "Juan Pérez",
    age: 55,
    introduceYourself : function(){
         alert("I'm " + this.fullName + " and I'm " + this.age + "years old");   
    }
    
}

person.introduceYourself();
    

 ===========================================

var Person = function(fullName, age){
this.fullName = fullName;
this.age = age;
this.sayHi = function(){
     alert("Hi!!");   
    }
}

var person1 = new Person("Juan Ramírez", 15);
console.log(person1);

var person2 = new Person("Oscar Victorín", 60);
console.log(person2);
person2.sayHi();

var person3 = new Person("Juan Rodríguez", 23);
console.log(person3);

var person4 = new Person("Mari Martínez", 35);
console.log(person4);

================================================

URL = 8fgbmusL    =   dbpzts4f (sintaxis corta)

var Person = function(params){
this.fullName = params.fullName;
this.age = params.age || "";
 
    }

Person.prototype.sayHi = function(){
    alert("Hi!" + this.fullName);
    
}

var people= [
    new Person({age: 10, fullName: "Juan Martínez"}),
    new Person ({fullName: "Pedro Garza", age: 10})
];

people.forEach(function(person){
    console.log(person);
});
