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
    
