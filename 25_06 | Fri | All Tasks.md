// Given URL: https://restcountries.eu/rest/v2/all




//------------------- Task 1----------------------
//Get all the countries from Asia continent /region using Filter function


  var xhr = new XMLHttpRequest();
  xhr.open("GET", "https://restcountries.eu/rest/v2/all");
  xhr.onload = function () {
    var data = JSON.parse(this.response);
    
    // Using filter funcion for filterout Asia region and getting their names using map
    
    var countriesnames = data.filter(x => x.region == "Asia").map(x => x.name);
      console.log(countriesnames);
    };
  xhr.send();
  
  
  
  
  
  
//-----------------Task 2----------------------
//Get all the countries with a population of less than 2 lakhs using Filter function



  var xhr = new XMLHttpRequest();
  xhr.open("GET", "https://restcountries.eu/rest/v2/all");
  xhr.onload = function () {
    var data = JSON.parse(this.response);
    
    //Using filter function to filterout population with given condition and getting their names
     
      console.log(data.filter(x => x.population <200000).map(x => x.name));
    };
    xhr.send();
  
  
  
  
  
 
//----------------Task 3-------------------
//Print the following details name, capital, flag using forEach function 
 
 
  var xhr = new XMLHttpRequest();
  xhr.open("GET", "https://restcountries.eu/rest/v2/all");
  xhr.onload = function () {
    var data = JSON.parse(this.response);
       data.forEach( x => console.log(x.name,x.capital, x.flag));
    };
    xhr.send();
    
    
    
    
    
//-----------Task 4------------------
//Print the total population of countries using reduce function 


  var xhr = new XMLHttpRequest();
  xhr.open("GET", "https://restcountries.eu/rest/v2/all");
  xhr.onload = function () {
    var data = JSON.parse(this.response);  
    let getSum = (x,y) => x + y.population;
      console.log(data.filter(x => x.population).reduce(getSum,0));
    };
    xhr.send();
    
    
    
    
    
// ----------Task 5------------------
//Print the country which use US Dollars as currency.



  var xhr = new XMLHttpRequest();
  xhr.open("GET", "https://restcountries.eu/rest/v2/all");
  xhr.onload = function () {
    var data = JSON.parse(this.response);  
      console.log(data.filter(x => x.currencies[0].symbol == "$").map(x => x.name));
      console.log(data)
  };
    xhr.send();
