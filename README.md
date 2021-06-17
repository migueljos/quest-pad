# quest-pad

//Q1
 var result = someFun({ someProperty: 'interview'}, function(value){
    
    console.log('This pointing to ' + value);

});

console.log('Result is', result);

function someFun(teste, teste2){
   
    teste2(teste.someProperty);
    return 1;
}


//QUESTÃO 2

var someFN = function(numero) 
    {
        var valor = numero;

        return function (incremento)
        {
            valor += incremento;
            return valor;
        }
    }

    var counter  = someFN(1)

    console.log("First call", counter(3))
    console.log("second call", counter(1))
    console.log("Third call", counter(5))

//Q3 
function calculator(val1,val2)
    {
        return function(callback)
        {
            return callback(val1,val2);
        };
    }

    var sum = calculator(1,2);

    sum(function (val1, val2) { return val1 + val2 });


 //Q4
/*
var a  = 5
var b = 10

if(a == 5){
  let a = 4
  var b = 1
  console.log(a)
  console.log(b)
}
console.log(a)
console.log(b)
//RESPOSTA: 4,1,5,1
*/



//Q5
/*
function multiplicar(numero)
{
     for(var i = 1; i < 10; i++)
     {
         console.log(i * numero)
     }
}
console.log(multiplicar(2))
*/
