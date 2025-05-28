# JavaScript Coading Practice 
## Arrays & Objects
### Js-1
    1) **Create And Log An Array**
    let arr = ['Orange',25,100,true,33.58]
    console.log(arr)

    2) **Acess the values of an Array**
    let index = parseInt(readLine());
    let myArray = [25, false, "green", "apple"];
    console.log(myArray[index])

    3) **Update the values of an Array**
    let index = parseInt(readLine());
    let val = parseInt(readLine());
    let myArray = [25, 50, "center", 75, 100];
    myArray[index] = val
    console.log(myArray)

    4) **Find the length of an Array**
    let input = readLine().replace(/'/g, '"');
    let myArray = JSON.parse(input);
    console.log(myArray.length)

    5) **Add the Value At end of the Array**
    let input = readLine().replace(/'/g, '"');
    let myArray = JSON.parse(input);
    let val = parseInt(readLine());
    myArray.push(val)
    console.log(myArray)

    6) **Remove the value at end of the array**
    let input = readLine().replace(/'/g, '"');
    let myArray = JSON.parse(input);
    console.log(myArray.pop())
    console.log(myArray)


### Js-2
    7) Call a Function
    function greet() {
      return "Hello! Have a nice day";
    }
    console.log(greet())

    8)Return the Value
    let firstInteger = parseInt(readLine());
    let secondInteger = parseInt(readLine());
    function getSumOfTwoIntegers(integer1, integer2) {
        return integer1+integer2
    }
    let sumOfTwoIntegers = getSumOfTwoIntegers(firstInteger, secondInteger);
    console.log(sumOfTwoIntegers);
    }

    9)Declare and Call the Function
    function getNationalBird(){
        return "Peacock"
    }
    let nationalBird = getNationalBird();
    console.log(nationalBird);

    10) Passing Argument to the function
    let personName = readLine();
    function greetWithName(personName) {
    let greetings  = "Hi " + personName;
    return greetings;
    }
    console.log(greetWithName(personName))

    11)create & call & Pass parameters to function
    let firstInteger = parseInt(readLine());
    let secondInteger = parseInt(readLine());
    function average(num1,num2){
      return (num1+num2)/2
    }
    let averageNum = average(firstInteger,secondInteger)
    console.log(averageNum)

    12)Create Function Expression
    let minutes = parseInt(readLine());
    let convertMinutesToSeconds = function(minutes){
      return minutes*60
    }
    let result = convertMinutesToSeconds(minutes);
    console.log(result);
