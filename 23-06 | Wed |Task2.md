//Problem 1

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var new_string = "";
 
for (var i = 1; i <= 11; i++) {
 new_string+= numsArr[i-1] 
}
console.log(new_string);




//Problem 2

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var new_string ="";
 
for (var i = 1; i < 11; i++) {
 new_string += numsArr[i-1] + ","
}
new_string += numsArr[10];
console.log(new_string);



//Problem 3

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var new_string = "";
 
for (var i = 11; i > 0; i--) {
 new_string += numsArr[i-1] + " ";
}
console.log(new_string.trim());




//Probelm 4

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
for (var i = 0; i <=10; i++) {
 if(numsArr[i] %2 == 0 )
 {
 numsArr[i] = "even"
 }
}
console.log(numsArr);




//Problem 5

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
for (var i = 0; i <=10; i++) {
 if(i%2 == 0 )
 {
 numsArr[i] = "even"
 }
}
console.log(numsArr);




//Problem 6

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var sum=0;;
for (var i = 0; i <=10; i++) {
 sum+= numsArr[i]
}
console.log(sum);




//Problem 7

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var sum=0;
for (var i = 0; i <=10; i++) {
 if(numsArr[i]%2 == 0)
 sum += numsArr[i]
}
console.log(sum);



//Problem 8

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var sum=100;
for (var i = 0; i <=10; i++) {
 if(numsArr[i]%2!= 0)
 {
 sum-= numsArr[i];
 }
 else
 {
 sum+= numsArr[i];
 }
}
console.log(sum);




//Problem 9

var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
for (var i = 0; i < numsArr.length; i++) {
 console.log( numsArr[i])
}




//Problem 10

var numsArr = [[1, 2, 3, 4, 5], [6, 7, 8, 9, 10, 11]];
var sum_odd = 0;
var sum_even = 0;
for (var i = 0; i < numsArr.length; i++) {
  var inner_array = numsArr[i];

  for (var j = 0; j < inner_array.length; j++) {
    if (inner_array[j] % 2 != 0) {
      sum_odd += inner_array[j];
    }
    else {
      sum_even += inner_array[j];
    }
  }

}
console.log(sum_odd);
console.log(sum_even);
