//Note:
//Used html comments for problem titles - for .html file errors and javascript comments for .js file errors



<!-- Problem 1 -->


<!DOCTYPE html>
<html>
<body>
 <script>
 alert( "I’m JavaScript!");
 </script>
 Whats the error in this ?
 <!-- Ans. Quotes  -->
</body>
</html>



// Problem 2 

//Quotes were different

alert("I’m invoked!");





//Problem 3


alert('Hello')  // JavaScript forgives if we not keep semicolon but keeping it makes your code a little easier to parse, and to compress.
alert(`Wor
 ld`) 		// These are template strings(i.e., backticks). No need of \n to create a new line sepearetly, it follow the string exactly the way it is)
 alert(3 +
1
+ 2); 		//Displays the expression output in dialog box




// Problem 4 

admin = fname+" " +lname;  //concatenate fname with a space and then with lname



//Problem 5

let name = fname+" " +lname;
alert( `hello ${name}` );



//Problem 6
let a = prompt("First number?");
let b = prompt("Second number?");
alert(+a + +b);



//Problem 7

var a = 2 > 12;
//Don't touch below this
if (a) {
  console.log("Code is Blasted")
}
else
{
  console.log("Diffused") 
}

//if numbers are compared as strings, "2" is bigger than "12", because "2" is bigger than "1". It returns true. So remove the quotes.





//Problem 8


Just press OK button when prompted. 'If condition' fails only at falsy values so inorder to make
'a' as falsy and go for else, we should enter nothing because return value is string we can't enter other falsy expressions.




//Problem 9

Just make "===" to "==" in "if" and "else if" statements. We know "===" operator checks type and value and "==" checks only value;



//Problem 10

let message = (login == 'Employee') ? "Employee" :
  ((login == 'Director') ? 'Greetings' :
  (login == '') ? 'No login' :
  '');
console.log(message);

//Added employee string wich was missing



//Problem 11


let message;
if (null || 2 || undefined )
{
 message = "welcome boss";
}
else
{
 message = "Go away";
}
  console.log(message);

//Removed the let keyword because it creates scope issue. Removing let helps in assigning the message




//Problem 12


let message;
let lock = 0;
//Dont change any code below this 
if (null || lock || undefined )
{
  message = "Go away";
}
else
{
 message = "welcome";
}
  console.log(message);

//lock is truthy value so changed the lock to 0 to make it falsy.



//Problem 13


let i = 3;
while (i) {
  console.log( i-- );
}



//Problem 14



let num = 1 ;
while(num <= 10){
  console.log(num);
  num++;
};


//Problem 15

for (let num = 2; num <= 20; num += 2) {
  console.log(num)
}


//Probelm 16

let gifts = ["teddy bear", "drone", "doll"];
for (let i = 0; i < 3; i++) {
  console.log(`Wrapped ${gifts[i]} and added a bow!`);
}

//Back ticks required




//Problem 17


let countdown = 100;
while (countdown > 1) {
  countdown--;
  if(countdown == 0)
  {
   console.log("bomb triggered");
  }
}




//Problem 18

It prints "hi"
0 is falsy but "0" is not falsy. String "0" is not empty so it is truthy. "If condition" fails at falsy statements.







