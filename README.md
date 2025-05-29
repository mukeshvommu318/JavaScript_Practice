# JavaScript Coading Practice 
## Arrays & Objects
### Js-1 [Arrays]
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

### Js-3 [object]
    1)Create & log Object
    let vehicle = {
    name:"Mercedes Benz",
    model:"C-Class",
    manufacturer:"Daimler AG company",
    length:"4686mm",
    "cargo capacity":"12.6 cubic feet"
    }
    console.log(vehicle)
    
    2)Create & log Object -2
    let movie = {
    title:"Baahubali",
    director:"Rajamouli",
    producers:['Sobhu','Raghavendra','Prasad'],
    "lead actors with their roles" : {
        prabhas:"Baahubali",
        anushka:"Devasena",
        rana:"Bhallaladeva",
        tamannah:"Avanthika"
        }
    }
    console.log(movie)

    3)Accessing the Object
    let objectKey = readLine();
    let person = {
    name: "Sam",
    age: 20,
    greet: function () {
      console.log("hello");
    },
    marks: {
      science: 70,
      math: 75
    },
    "languages known": ["telugu", "hindi", "english"]
    };
    console.log(person[objectKey])

    4)Modifiy the object
    let objectKey = readLine();
    let val = JSON.parse(readLine().replace(/'/g, '"'));
    let cat = {
    name: "lizzie",
    age: 18,
    "fur color": "grey",
    likes: ["catnip", "milk"],
    birthday: { month: 7, day: 17, year: 1994 }
    };
    cat[objectKey]=val;
    console.log(cat)

    5)Add the new element to Object
    let objectKey = readLine();
    let val = JSON.parse(readLine().replace(/'/g, '"'));
    let meals = {
    breakfast: "Oatmeal",
    lunch: "Burrito",
    dinner: "Chapathi"
    };
    meals[objectKey]=val
    console.log(meals

    6)Make a person Object
    let id = parseInt(readLine());
    let name = readLine();
    let email = readLine();
    function makePersonObject(id,name,email){
      let person ={
          "id":id,
          "name":name,
          "email":email
      }
      return person
    }
    let personObject = makePersonObject(id, name, email);
    console.log(personObject);

    7)Find the Total Score [10,20,30]
    let arrayOfScores = JSON.parse(readLine().replace(/'/g, '"'));
    function calculateTotalScore(arrayOfScores){
      let [first,secound,third]=arrayOfScores
      let totalScore=first+secound+third
      return totalScore
    }
    let totalScore = calculateTotalScore(arrayOfScores);
    console.log(totalScore);

    8)Make an array 1,2,3
    let num1 = parseInt(readLine());
    let num2 = parseInt(readLine());
    let num3 = parseInt(readLine());
    function makeAnArray(num1,num2,num3) {
       return [num1,num2,num3]
    }
    let createdArray = makeAnArray(num1, num2, num3);
    console.log(createdArray);

    9)Eligibilty to play the next level of the game /{'name':mukesh,'score':4}
    let person = JSON.parse(readLine().replace(/'/g, '"'));
    function isEligibleForNextLevel(person) {
     if(person['score'] > 5){
         return true
     }
     else{
         return false
     }
    }
    let isPersonEligible = isEligibleForNextLevel(person);
    console.log(isPersonEligible);

    10)Game Mode /['muk']
    let arrayOfFriends = JSON.parse(readLine().replace(/'/g, '"'));
    let noOfFriends = arrayOfFriends.length
    function getPreferredGameMode(noOfFriends){
      if(noOfFriends===0){
          return "Solo"
      }
      else if(noOfFriends===1){
          return "Dual"
      }
      else{
          return "Squad"
      }
    }
    let gameMode = getPreferredGameMode(noOfFriends);
    console.log(gameMode);

### OwnPractice - 1
    1) How to Access the value : Array(object(value))
    let todoList = [{text : "learn html"},{text:"learn css"}]
    console.log(todoList[0].text)

    2) Button Click Function Expression 
    <!DOCTYPE html>
    <html>
      <head></head>
      <body>        
        <h1 id="heading">Baseball</h1>
        <button onclick="changeHeading()">Change Heading</button>
      </body>
    </html>
    let changeHeading = function() {
      document.getElementById("heading").textContent = "Cricket";
    };

    3)Adding the elements using JavaScript
    <!DOCTYPE html>
    <html>
      <head></head>
      <body>
        <div id="bgContainer"></div>
      </body>
    </html>
    let myContainer = document.getElementById('bgContainer');
    let technologiesArray = ["Artificial Intelligence", "Virtual Reality"];

    function createAndAppendTechnology(technology){
      let technologyItem = document.createElement("p");
      technologyItem.textContent = technology;
      myContainer.appendChild(technologyItem);
    }
    
    for(let technology of technologiesArray) {
      createAndAppendTechnology(technology);
    }

### Js-5
    1) Summ of the values of the Array
    let myArray = JSON.parse(readLine().replace(/'/g, '"'));
    let sum =0
    for (let eachitem of myArray){
          sum = sum+eachitem
    }
    console.log(sum)

    2)Log the Values of each Object
    let objectKey = readLine().replace(/'/g, '"');
    let arrayOfInventions = [
    {
      name: "Printing Press",
      "invented by": "Johannes Gutenberg",
      year: 1440
    },
    {
      name: "Light Bulb",
      "invented by": "Thomas Edison",
      year: 1879
    },
    {
      name: "Telephone",
      "invented by": "Alexander Graham Bell",
      year: 1876
    },
    {
      name: "Aeroplane",
      "invented by": "Orville and Wilbur Wright",
      year: 1903
    },
    {
      name: "Computer",
      "invented by": "Charles Babbage",
      year: 1822
    }
    ];

    for (let eachitem of arrayOfInventions){
        console.log(eachitem[objectKey])
    }

    3)Eligibility to vote   i/p : [{'name':"mukesh",'age':34},{},{},...]
    let arrayOfPersons = JSON.parse(readLine().replace(/'/g, '"'));

      for (let each of arrayOfPersons){
          if(each['age']>=18){
              console.log(each['name'])
          }
       }

     4)
