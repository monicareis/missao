document.getElementById("calculate-button").onclick =function() {
 
 //Coletar números dentro das caixas de input
 let elem1 = document.getElementById('elem-1');
 let elem2 = document.getElementById('elem-2');
 let val1 = parseInt(elem1.value);
 let val2 = parseInt(elem2.value); 
 
 if (!val1) {
  alert('Digite valor na primeira caixa!');
  elem1.focus();
  return;
 }

 if (!val2) {
  alert('Digite valor na segunda caixa!');
  elem2.focus();
  return;
 }

 let choice= document.querySelector('input[name="operation"]:checked');
 let operation= choice.value;
 let operationResult= getResult(val1, val2, operation);
 let resultElement= document.getElementById('result');
 resultElement.innerHTML= operationResult; 
 }
    /**
    *Returns the result of an operation over two numbers.
    *Arguments: two valid numbers and one operation symbol.
    *Supports sum, subtraction, multiplication and divison.
    */
function getResult(val1, val2, operation) {
 if (operation === "+") {
  return val1 + val2;
 }
 else if (operation ==='-') {
     return val1 - val2;
 } 
 else if (operation ==='*') {
        return val1 * val2;
 } 
 else if (operation ==='/') {
  return val1 / val2; 
 }
 else if (operation ==='%') {
  return (val1 * val2)/100; 
    } 
 else if (operation ==='^') {
  return Math.pow(val1, val2);
 }  
}
