# Coder Academy - Workbook
## Assignment 1 - Term 3 (T3A1)

## Question 1
Provide an overview and description of a standard source control process for a large project

Source control, is a project management process and tool, used to track and manage code changes and updates. At their core, Source Control Management software like CVS, Monotone and most popularly Git, provide a way for users to track a running history of their code, allowing them to access past changes and manage their code by segmenting it into separate versions, helping the user control the workflow and merge potential project features without the risk of conflict changes to the main code.

Source control is helpful for managing a single users code, but necessary when it comes to managing a group project or code with multiple contributors. Source control allows a safe environment for each contributor to update and add code without conflicting edits. According to Bitbucket, before source control management, developers would edit text files directly and move them around to remote locations using FTP and or other protocols. Often, a developer would make edits and another developer would unknowingly save over their work, wiping out any changes. 

Now, with the help of Source Control Management tools, code changes from each individual are tracked and the SCM software identifies conflicts in code and warns the developer. Allowing each contributor to commit and merge smaller code blocks like feature updates, without conflicts to the main source code.

As mentioned above, Git is the most popular source control tool; one key aspect of source control and Git, is working with branches. By default, a projects main source code is saved on the main/master branch, and is where all the final code will be pushed to. When working as a group, each individual will create a new branch to work from. This branch is separated from the main branch, allowing a developer to have their own commits and pushes. Working from a branch to update code changes or add new features is important so not to compromise the main source code.

Once a feature has been completed, the developer will merge and push their code to the main/master branch.

See appendix


https://homes.cs.washington.edu/~mernst/advice/version-control.html
https://www.mathworks.com/help/simulink/source-control-in-simulink-project.html
https://www.atlassian.com/git/tutorials/source-code-management
https://homes.cs.washington.edu/~mernst/advice/version-control.html




## Question 2
What are the most important aspects of quality software?

*List discuss and demonstrate 6 software quality characteristics.*

There are detailed metrics that outline the quality of software. Quality of software is not only related to the function of the software itself but also the function of the software and its purpose. 

6 aspects of quality software

Code Quality – The quality of code is determined by the both quantitative and qualitative metrics. To quantify the quality of code we look at metrics like Big-O complexity, length of code, types of functions, code structure, bug-free and refactored. Qualitative measures of code include readability, maintainability and code efficiency.

Reliability – Reliability is a measure of failure-free runtime across different conditions and environments. Reliability can be measured using the Mean time between failures (MTBF) equation which is “the predicted elapsed time between inherent failures of a mechanical or electronic system, during normal system operation” (Wikipedia). By analyzing the number of failures, errors or defects,  we can measure how well the software works and how long the system will run smoothly without crashing. If errors do occur, the reliability of software is also measured by how these errors are handled especially from the perspective of the user and the purpose of the software.

Testability - Testability determines how a software is tested to validate its effectiveness, catch errors and prove an efficient user experience. Testability or the methods for testing software should be easy. To do this the best methods are implemented early in a project and should include a comprehensive automated test suite. 


Security - Software security is important to ensure safe and secure handling of data on both the user and the developer side. Without the proper security measures in place, a company is prone to malicious attacks and potential data breaches. Data security should be a high priority focus for a developer of company as there could be potential legal repercussions if not handled correctly, and the reputation of the entity is at stake. Following proper security protocol when working with API's and keys, payment keys and user info is important at all stages of development and should be tested/checked regularly even if there are no changes to the code or software. 

Usability - Usability refers to the ease of which users can execute tasks within a system. The user journey is key to the measure of usability; this includes how the UI responds, how errors are handled, the ability for a user to navigate a system and the user return/retention rate. If the user journey is confusing, resulting in high usage of support channels and ultimately disuse of the system, the software needs to be reviewed and updated. Quality Assurance engineers test software to ensure the highest level of usability from beginning to end with a focus on updates throughout the software lifecycle. This includes accessibility features built for people with disabilities.
 
Maintainability - Maintainability refers to the methods by which a code is maintained and updated; maintainability is crucial to longevity. Although unlike hardware, software may not deteriorate physically, but given the purpose of most software applications it should evolve and meet ever changing requirements of the developing entity and the user. As time goes on, software will go through cycles of change to implement and update new and existing features. If code is not maintainable, a company or entity will have to commit huge resources into these changes. 



## Question 3
Outline a standard high level structure for a MERN stack application and explain the components

*Shows almost flawless understanding of the high level structure of the app*

The two most popular tech stacks for JavaScript based development projects are MERN and MEAN stacks. 

MERN is an abbreviation for the 4 main technologies that make up the stack which are MongoDB, Express, React, and Node.



MongoDB - document database
Express(.js) - Node.js web framework
React(.js) - a client-side JavaScript framework
Node(.js) - the premier JavaScript web server

MongoDB is a NoSQL database solution built on either MongoDB servers of hosted on third-party services. Unlike traditional relational databases where information is broken up into tables and stored as separate but related entities, Mongo uses a document model. MongoDB replaces relational database tables and rows with documents that have a similar structure to Javascript objects or JSON files and allows a developer to work objects and arrays while using a single record; the document model is also schema free.
To understand Express.js we first need to understand node.js. Node.js is a cross-platform runtime environment for executing JavaScript code outside of the browser and is often used for back-end development, especially when working with API’s. Node.js is a popular runtime environment as it allows for fast and highly scalable services and apps, while following the principles of agile development. 
Express.js is a web framework for Node.js. A web framework is a pre-structured simplified process to building web applications. Just like Rails, Express relies on built in methods to manage http requests and routing easily and quickly. Not only does Express help to simplify the code used for these requests, but also help organize the application into MVC architecture.
React.js was developed by Facebook in 2011 and is one of the most popular JavaScript libraries. JavaScript libraries assist developers by creating pre-packed methods and code snippets mitigating the need to reuse the same code over and over thus speeding up development and simplifying code. React is a library built on components which are portions of the User Interface broken up into smaller reusable code. These components are part of a larger tree of components and can be used over and over to build complex web apps and detailed user interfaces. 
These technologies interact with each other to create and display web apps and work on both the client side, and the server side. On the client side we use React to present data and information to the user including updating the user interface, validating user input and showing feedback to the user and everything else that the user sees on their screen. In traditional web apps the client or browser fetches a new HTML page for every click as the browser is updated but React uses Single-Page-Application development which updates the existing page; rendering new JavaScript in the UI when needed.
The server side of a MERN stack application is where we use Node.js, Express and MongoDB to manage application logic that is hidden from the user/browser like authentication logic, or logic that is too large or heavy to run in the browser, as well as any data such as files or databases. Although MongoDB sits in a separate server from Node.js and Express, theses technologies are used to talk to the Mongo database and relay the information to the client.
The client side and the server side communicate through requests and responses but because we build the front end as a single page application, when we send a request it is sent in the background which does not request a new HTML page and re-renders, but instead requests data to update and manipulate the existing HTML page with the help of JavaScript and React.


https://www.mongodb.com/mern-stack
https://medium.com/codingthesmartway-com-blog/the-mern-stack-tutorial-building-a-react-crud-application-from-start-to-finish-part-2-637f337e5d61
https://www.geeksforgeeks.org/mern-stack/



## Question 4
A team is about to engage in a project, developing a website for a small business. What knowledge and skills would they need in order to develop the project?

##### Communication and planning

Communication is an important part of any team, but especially for a team of developers. 
From start to deployment to testing, if communication is not clear, concise and consistent, a project will fail. The gold standard for software development in 2021 are AGILE project management strategies. Agile is an iterative project management method that utilizes short 
"sprints" to accomplish realistic and user focused goals.

Each day through Scrums or stand-ups a team can communicate accomplishments and challenges from the previous sprint and plan the goals for the next spring with the team. This approach enables each team member to effectively work on their individual projects knowing what others are doing and gives them an insight into what could come up in terms of errors and conflicts in code, and also the changes that will be implemented in sources code. 

##### Testing

Understanding the proper techniques and methods for software testing is a key part of team development projects. A team will have to decide on what testing automations to build and use, and how often these tests will be run. There could be an individual assigned to test other team members software, or an agreement for each member to utilize TDD or test driven development where they write their own tests for each function and feature they're working to implement. 

##### Customer requirements

For any project to succeed a team needs to know the project requirements and in this case, those requirements come from the client. Understanding the clients needs is key to producing a quality shipped product and to do so, the team must understand what the client is looking for and to meet their expecations.

###### Timeline
Understanding the clients timeline will help with project planning, feature releases, the completion of a minimum viable product and so on. If we understand the timeline for each phase, feature build, source code update etc. As developers, we will be better enabled to manage the product and the expectations of the client without being overwhelmed, mitigating the likelihood of delivering a prompt shippable product.

###### Milestones
Working in cooperation with the client to set timelines is important, but there also needs to be consistent physical updates for the client to see and give feedback on. Setting milestones with the clients, or dates to update them on the project is an important part of the process.


##### Tech requirements

Understanding the tech requirements to fit the customer requirements is also an important piece of the puzzle. 

- Hosting Infrastructure
This refers to how the site and its data will be hosted so that it can be displayed on the internet and includes the domain, hosting, file storage and CDN caching. Hosting infrastructure can be expensive - having the knowledge on what to recommend the client is key to budget planning and limiting high project costs. 


- Tech Stack
It's imperative to understand what tech stack to use; a tech stack that's good for the client and specific project, but also good for the developers. Utilizing known tech stacks is obviously the most effective and efficient way to build a website, but if the client has an opinion that differs, are we able to adapt, or are we not the right fit for the client?
Choosing the right tech stack and having the skills to sell the different tech stacks to the clients is key to helping them understand a stacks capabilities so that the project has realistic expectations for the final product, and its features.


##### Git

Source control is helpful for managing a single users code, but necessary when it comes to managing a group project or code with multiple contributors. Source control allows a safe environment for each contributor to update and add code without conflicting edits. According to Bitbucket, before source control management, developers would edit text files directly and move them around to remote locations using FTP and or other protocols. Often, a developer would make edits and another developer would unknowingly save over their work, wiping out any changes. 



## Question 5

*With reference to one of your own projects, discuss what knowledge or skills were required to complete your project, and to overcome challenges*

The Ruby on Rails project was challenging and I had to learn many new skills and gain a lot of knowledge to complete it. 

###### Application Framework

This project was the first experience I had with working with web and application frameworks. Knowledge of the MVC architecture of a framework when undergoing this project was one of the most important aspects. While frameworks like the one we used, Rails, exist to make web application development easier and more efficient, it was a steep learning curve to understand how the components interact and fit together. For example, one of the most challenging concepts to grasp was the interaction of each stage in the MVC architecture. Understanding the basics of MVC is easy enough, but when you're writing source code it is difficult to track what data is transferrable and reusable across each of the components including how classes interact with each other, and how information is accessed using different routes and different components of MVC.


###### Databases and backend

Working with databases and entity relationships; schema designs, Postgresql, Active record, Migrations etc. Lot's to know, and lot's to understand. Knowledge of these concepts was crucial to completing the project. I had to overcome the challenge of no prior knowledge in order to effectively implement and manipulate different data and entities while integrating this knowledge with the skill to navigate the MVC structure. Understanding how databases are created, manipulated and stored is key to providing a shipped useable product.  

###### Time Management
Time management is a useful skill to have when undertaking a programming project. Time management in development can be challenging as a sprint, or focus on a specific feature is never 100% calculable. To address time management issues I set achievable goals based on: adding features, adding entities, creating and updating functions, and also learning. I set time frames to learn new topics and theories or else I would get overwhelmed by related topics.

some other ways to manage time in a development project are to:

- plan and prioritize tasks
- adjust priorities 
- set realistic goals for minimum viable products
- split tasks into bite size sprints


###### Git and Github
Source control was helpful for managing updates to my source code. It was challenging however as it was the first real project I undertook and so had to learn to use Git and Github on a larger scale. 




## Question 6
*With reference to one of your own projects, evaluate how effective your knowledge and skills were for this project, and suggest changes or improvements for future projects of a similar nature*

I didn't feel that my knowledge and skills were up to par for the project I had to undertake. During the process I found myself spending more time on learning, and relearning concepts than putting the concepts in to practice. While implementing concepts in a code project there will always be a need to learn and adapt, but in the future, I think I can minimize the learning curve by first planning what concepts are need in the project, and how they relate to each other.

For example, before the project started I didn't have a good grasp on the concept of ActiveRecord and didn't know the purpose or use case for it. When it came time to implement the concept I spent more time trying to understand it than use it; in addition to that I didn't know how the concept influenced or related to each stage of the project.

Another change I would make is the in the planning stage for project features. Before this project started I didn't have a clear detailed picture of the features I wanted to implement. I thought I knew what features would be nice to have, but didn't understand how realistic they were. When it came time to implement or build a feature, I felt overwhelmed by the task and settled with a very different final product.

## Question 7
*Explain control flow, using an examples from the JavaScript programming language*


By default, Javascript code is executed from top to bottom, line by line; however, we can change the sequence with control flow. Control flow allows a program to make decisions about what code, and when it is executed.

#### Conditional statements and loops

Conditional statements work on the premise that there are always cases in programming where a task is executed based on certain conditions. Conditional statements represent a foundation to the JavaScript language and can be written in different methods and flows.

##### if...else if...else

If statements are the base of conditional statements of most programming languages. While some languages have different syntax, all languages utilize these basic conditional statements.

```js
const array = ['blue', 'red', 1, true];
if( array.length == 5){
  console.log("There are 5 elements in this array");
} 
else if (array.length < 5){
  console.log(`There are ${array.length} elements in this array`);
}
else {
  console.log("Too many elements in the array");
}
```

In the above example the if statement does not execute because it does not pass the conditional. Instead the second conditional of the ```else if``` runs and prints ```There are 4 elements in this array``` to the console. This is an example of control flow.


##### Switch statements 

Switch statements executes similar to a longer if/else chain. The switch expression is executed when the value of ```switch``` is compared against the values of each ```case```. When a case is found to be ```true```, the code block in that statement will execute.

```js

function moods(mood) {
  switch(mood){
    case "happy":
    console.log("Dance to Pharrell's Happy");
    break;
  case "sad":
    console.log("You should eat a pint of ice cream");
    break;
  case "anxious":
    console.log("Take some deep breaths");
    break;
  case "hungry":
    console.log("You should eat a big chocolate cake");
    break;
  default: 
    console.log("That's not a mood we support");
  }
}

moods("anxious");
```
This function prints ```Take some deep breaths to the consoled``` as the ```case``` of ```"anxious"``` is passed and found to be true. When the case is evaluated as true, the program ```breaks``` out and executes the block of code associated with the true case.


##### Error handling

Another important aspect of control from is error handling for usability and testability for the developer and the user. One method to handle errors is a ```try..catch``` statement. This statement will evaluate a block of code or ```try``` to run and if found true execute the associated code block, if found to be false the statement will ```catch``` the error and execute a different block of code. As well as ```try``` and ```catch``` a third and final statement will always run, this is called ```finally```.

```js
const checkName = name => {
  try{
    let length = name.length;
    if (length < 10){
      console.log("Good name")
    } else {
      console.log("Very Goood name");
    }
  } catch (err){
    console.log("Please pass a name");
  }
  finally{
    console.log("This statement will run no matter what")
  }
}

checkName("Jordan");
checkName();
```

This code first runs the ```if...else``` statement in ```try``` to make a logical comparison of the length of ```name```. When found to be true, the ```try``` block will execute. If however the try block can not be executed, like in the code above if ```checkName()``` is missing a parameter, the ```catch``` block will execute. The ```finally``` block executes no matter which statement or block is executed.

##### Callbacks
According to wikipedia a callback is "any executable code that is passed as an argument to other code that is expected to call back (execute) the argument at a given time." We can also understand callbacks as functions that execute after, or as a product of another function being called. This ```callback``` is often passed as the parameter to a higher order function (a function that accepts another function as a parameter)

```js
const getDressed = callback =>{
  callback();
  console.log("put on pants")
  console.log("put on top")
}

function underwear(){
  console.log("put on underwear")
}

getDressed(underwear);
```
This code gives the ```getDressed``` function ```underwear``` as a callback and executes the code block when it is called within the function. The sequence executes in the intended order. Callbacks are useful for tasks like retrieving information from a database to return to the user. Because the program waits for a callback function to execute before running the next line of code (as seen in the example above).


Callbacks however have nesting and runtime issues creating pitfalls in efficiency. When we run callbacks we have to wait for the code to run to move on to the next line of code. If we are iterating through a database then the function may take longer to run depending on the size of the database. To solve these issues we use an asynchronous method called ```promises```. 

##### Promises

Promises in JavaScript are asynchronous ways to call a function with a ```promise``` as a placeholder for a value to return. While these promises are running they are in a "pending state" and the program continues to run under the ```promise``` of returning a value sometime in the future. The ```promise``` eventually returns a ```resolve``` or ```reject``` value  and then calls the callback functions ```then``` and ```catch```.

```js
const fs = require('fs')

const getFile = (fileName) => {
  return new Promise((resolve, reject) => {
    fs.readFile(fileName, (err, data) => {
      if (err) {
        reject(err)  // this will cause the promise to fail 
        return        // break out of execution
      }
      resolve(data)
    })
  })
}

getFile('/etc/password')
.then(data => console.log(data))
.catch(err => console.error(err))
```

In this code we are creating a ```promise``` to read a file, passing it ```reject``` and ```resolve``` callback functions. The ```promise``` will  run in a pending state while other code is being executed. Once the promise has finished running, it will return either the ```reject``` or the ```return``` block as callbacks and give access to those values to call in ```then``` and ```catch``` statements.


##### Asnc/await

```Async``` functions along with eh ```await``` keyword were released in 2017 and is the newest addition to asynchronous control flow in JavaScript. While the method works fundementally the same as ```promise```, the syntax and return statements are placed to make the code shorter and more readable. ```async```/```await``` is often used in a similar scenario as above to fetch data from a database, or an API.

```js

async function getUsers(url){
  try{
    let response = await fetch(url);
    let data = await response.json();
    console.log(data);
    return data;
  }catch(err){
    console.log(error);
    return err;
  }
}

```
The above code is a simple example of fetching data using an ```async``` function. You'll notice that the need for ```then``` and ```catch``` callbacks are not longer needed, making the code more efficient and maintainable. It also shortens the main block of code by setting varibales for ```response``` and ```data``` inside the function to then use and return the values. 


## Question 8
Explain type coercion, using examples from the JavaScript programming language


##### Implicit and explicit
Every operation in JavaScript is is built by evaluating different data types. Every function or method expects a certain data type of value in order to correctly run the code and return the desired value. There are rules outlining what values can be interpreted against another but some of these rules are handled by JavaScript.

```js
let myNumber = 3; //this statement has a typeof number
let myString = "4"; //this statement has a typeof string

console.log(myNumber * myString);
```
The code above for example prints ```12``` to the console, even though we are multiplying a ```string``` with a ```number```. JavaScript automatically converts the typeof string to a number so that it can evaluate the operation; this is implicit type coercion. Type casting, or explicit type coercion on the other hand is different in that the developer explicitly tells the program what data type to compare and convert. This is done using built in methods like ```String()```, ```Number()```, and ```Boolean()```.

```js
Number("42"); // returns 42
String(42); // returns "42"
Boolean(0); // returns false
```

The code above returns the conversion of the ```string``` ```"42"``` to a ```number```, the ```number``` ```42``` to a ```string```, and ```0``` to a boolean.


##### Strict and loose equality

Loose and strict equality refers to how a program compares two values. Loose equality allows for type coercion where strict equality does not. A developer can use loose equality to check if two values are equal, if the value data types are not the same, javascript with coerce the data to compare and return a result.

Strict equality on the other hand is a direct comparison of value and type, JavaScript will not attempt to coerce these data types and only return a result as ```true``` if both conditions are true, otherwise it will return ```false```.

Loose equality
```js
0 == false // true (0 is falsy value) - coerced to false == false
15 == '15' // true - coerced to '15' == '15'
null == undefined // true - coerced to false == false
```

Strict equality

```js
0 === false // false - number is not a boolean
'15' === 15 // false - string is not a number
null === undefined // false - null is not undefined
```



## Question 9
### Explain data types, using examples from the JavaScript programming language



Data types in JavaScript include strings, numbers, booleans, undefined and null. These data types are referred to as primitive and are immutable or unchangeable, while objects and arrays are mutable and considered 'Special'. While special data types have properties and methods standard to their structure, primitive data types are "wrapped objects", meaning they also have methods first they must be 'wrapped' as an object to do so, this wrapping is handled by JavaScript. 


### Primitive Data Types 

```undefined``` : The undefined data type is a "non-configurable, non-writable property". Variables that have been declared but NOT assigned a value have a type of ```undefined```. A function returns an ```undefined``` data type if a value is not returned. Other examples include an array index or object property that does not exist or a function parameter that is not supplied.

```
const findLastIndex = (array, needle) => {
  array.forEach((el, i) => {
    if(Object.values(el).includes
    (Object.values(needle)[0])){
      return i;
    }
  })
}
```

This code returns ```undefined``` as .forEach() does not return a custom statement.

```string```: The string data type is used to represent text data or a sequence of characters. String data types are created using single or double quotes ('example', "example"). Unlike Ruby, an empty string ('', "") in JavaScript will return undefined. 

```console.log(typeof 'string example')``` and ```console.log(typeof "another example")``` will both return ```string```.

Strings can also be manipulated using concatenation and interpolation using the ```+``` symbol, and ```${}```. For example:
```"My name is" + " Jordan"``` returns ```"My name is Jordan"```. ``` let name = "Jordan" `My name is ${name}` ``` also returns ```"My name is Jordan"```.

```number```: Unlike other programming languages, JavaScript has the same data type for all number formats. In other languages numbers with a decimal point are interpreted as floating-point values, and those without as integers. JavaScript interprets both as numbers. 

``` console.log(typeof 5)``` returns ```number``` and ``` console.log(typeof 0.5)``` also returns ```number```.

```boolean```: Boolean data types have two values, ```true``` and ```false```. Boolean values can be used to determine if an operation is true or false, and often used to determine a 'yes' or 'no' answer to conditional operations and statements. 

```let yes = true;
let no = false;

if(yes){
  console.log("This code will be executed");
}

if(no){
  console.log("This code will not be executed");
}
```

```null```: Null is a data type that represents nothing, or that something has 'no value'. In programming regular english expression such as ```0``` still has a value (```console.log(typeof 0)``` will return ```number```). The same case stands for ```undefined```, where undefined does not indicate no value, but that the value exists, but is undefined. ```null``` however represents a data type of nothing, or no value. ```null``` is special though in that when testing the typeof (```console.log(typeof null)```) it will return an 'object'. This is because ```null``` is part of the 'object-type primitive subtree, not an instance of an object.


```
const getVowels = string => {
  const m = str.match(/[aeiou]/gi);
  if (m === null){
    return 0;
  }
  return m.length
}

console.log(getVowels('sky'));
```

This will return ```0``` as the if statement is true, there are no vowels found in the ```"sky"``` string parameter and returns a ```null``` value, or nothing. 


### Special/Complex Data Types

Objects are considered special or complex data types with direct properties and methods, Arrays in JavaScript are also technically objects, or a list of object properties.

Objects contain properties defined as key-value pairs. Object keys or key names have to be strings, numbers, or symbols while an object value can be any type. 

```
let emptyObject = {};
let carObject = {"make": "BMW", "year": 2019, "available": true}

```

Arrays are also special or complex data types and are used to store lists of values. Each value is referred to as an element and is assigned a numbered index starting at ```0``` for the first element in the array. Arrays have no limit to what values it can hold and they can be of any data type including nested arrays, and objects.

```
let sports = ["Soccer", "AFL", "Weightlifting"];
let randomList = ["Building", 1, true, .95, {"name": "Jordan", "age": 33}];

```


## Question 10
*Explain how arrays can be manipulated in JavaScript, using examples from the JavaScript programming language*


Like mentioned above, Arrays are just objects and objects are mutable; they can be mutated or changed. An array never has an end point and can always be updated, added to or subtracted from. Every Array has an index assigned to each element, or value in the list starting at ```0```eg. ```let array = ["car", "person", "shoe"]``` Car has an index of ```0```, person ```1```, and shoe ```2```.

In order to efficiently manipulate arrays, JavaScript has a built in methods that we can call on an array and even chain together. While there are close to 50 built in array methods in JavaScript, some of the important ones are listed below.


##### Array Index
- Accessing a single element in an array is done so by referencing the elements index.

```
const cars = ['BMW', 'Toyota', 'Mazda'];
const car = cars[1];
console.log(car);

```

This prints ```'Toyota'``` to the console.

##### ```.length```
- This method uses the above index count of array elements and returns the number of elements in an array.

```
const cars = ['BMW', 'Toyota', 'Mazda'];
const car = cars.length;
console.log(car);
```

This prints ```3``` to the console

##### ```.map()``` 
- creates and returns a new array with the value of the result of calling a function on every element in the array. The elements in the new array are mutated.

```
var arr = [{
    name: 'Thomas',
    age: 19},{
    name: 'Jordan',
    age: 17},{
    name: 'Luc',
    age: 20}]

console.log(arr.map(function(element){
    element.age += 1    
    return element
}))
```

This returns a new array with the age key-value pair incremented by ```1``` eg. ```{name: 'Thomas', age: 20}```.

##### ```.filter``` 
- creates and returns a new array with all elements that pass a condition. Unlike ```.map()```, ```.filter()``` does not return mutated elements, but returns a new array with elements from the original array.

```
const condition = human =>{
  return human.age <= 18
}

let arr = [{
  name: 'Jordan',
  age: 18},
  {name: 'Sarah',
  age: 13},
  {name: 'James',
  age: 25}]

  console.log(arr.filter(condition))
```
This example will return the Jordan and Sarah elements, which are objects.

##### ```.find()``` 
- returns the first element that passes a condition. If no element passes, the method will return ```undefined```

```
const condition = human =>{
  return human.age >= 18
}

let arr = [{
  name: 'Jordan',
  age: 19},
  {name: 'Sarah',
  age: 18},
  {name: 'James',
  age: 25}]

  console.log(arr.find(condition))
```
This example returns element at index ```0``` as it is the first element, or object that passes the condition. 


##### ```.forEach()``` 
- is an iteration method that loops over every element in an array without mutating the array. forEach often returns a callback function like the below example:

```
const colors = ['blue', 'green', 'orange'];

const iterate = item => {
  console.log(item)
}

colors.forEach(iterate)
```

This returns each element in the colors array using the ```iterate``` function as the callback, looping and calling the function on each element in the array.

##### ```.includes()``` 
- This method checks if an element in an array passes a condition and returns true or false.

```
const arr = [1, 'blue', 8, 'car', true];

console.log(arr.includes('blue'));
```

The ```console.log()``` statement will print ```true``` to the console as ```'blue'``` is found in the array.


##### ```.push()```
- This method adds one or more elements to the end of an array and returns the length of the new array. The original array is mutated and can be returned.

``` const sports = ['soccer', 'golf', 'AFL'];
const count = sports.push('rugby');
console.log(count);
console.log(sports)
```

This prints ```4``` and ```['soccer', 'golf', 'AFL']``` to the console.

##### ```.pop```
- This method is the opposite of push and removes an element from the end of an array and returns the element that is removed.

``` const sports = ['soccer', 'golf', 'AFL'];
const count = sports.pop();
console.log(count);
console.log(sports)
```

This prints ```AFL``` and ```['soccer', 'golf']``` to the console.


##### ```.shift()```
- This method removes the element at the beginning of an array and returns the element. 

``` const sports = ['soccer', 'golf', 'AFL'];
const count = sports.shift();
console.log(count);
console.log(sports)
```

This prints ```'soccer'``` and ```['golf', 'AFL'] to the console


##### ```.unshift()```
- The opposite of shift where the method add an elements to the beginning of an array and returns the new length of the array.

``` const sports = ['soccer', 'golf', 'AFL'];
const count = sports.unshift('rugby');
console.log(count);
console.log(sports)
```

This prints ```4``` and ```['rugby', 'soccer', 'golf', 'AFL'] to the console



## Question 11
Explain how objects can be manipulated in JavaScript, using examples from the JavaScript programming language

Objects are considered special or complex data types with direct properties and methods, Arrays in JavaScript are also technically objects, or a list of object properties.

Objects contain properties defined as key-value pairs. Object keys or key names have to be strings, numbers, or symbols while an object value can be any type. 

```
let emptyObject = {};
let carObject = {"make": "BMW", "year": 2019, "available": true}

```

A JavaScript object has properties which are like variables to the object, variables that store specific values attached to objects: Object properties can be accessed with dot-notation: 

```objectName.propertyName```

``` 
const myCar = {
  make: 'Toyota',
  model: 'Land Cruiser',
  year: '1988',
  color: 'White'
}
```


To manipulate Objects we first need to understand property accessors. There are two ways to access JavaScript Object properties; dot and bracket notation.

#### Bracket-notation: 

```
const animalSound = {
  cat: 'meow',
  dog: 'woof'
}

let sound = animalSound['cat'];
console.log(sound);
```
This prints ```meow``` to the console.

#### Dot-notation: 

```
const animalSound = {
  cat: 'meow',
  dog: 'woof'
}

let sound = animalSound.dog;
console.log(sound);
```
This prints ```woof``` to the console.

#### Object Enumeration

There are native methods to use object enums in JavaScript and traverse, list and loop over Objects.

##### ```for...in```

- This method loops/iterates over enumerable properties in an object. It does not however loop over symbols, only keys that are strings.

```
var car = {
   maker: "honda",
   color: "blue",
   type: "sedan",
   mpg: "32"
}
 
for (var prop in car){
console.log( "The " + prop + " of this car is: " + car[prop] );
```

##### ```Object.values()```
- This method returns an array of the values of an object. 

```
const user1 = {
  age: 33,
  mobile: 0400088883,
  name: "Jordan"
}
const user = Object.values(user1);
console.log(user) //[33, 0400088883, "Jordan"]
```

##### ```Object.keys()```
- This method returns an array of the keys of an object.

```
const user1 = {
  age: 26,
  mobile: 8801967402131,
  name: "Talha"
}
const user = Object.keys(user1);
console.log(user) //["age", "mobile", "name"]
```

##### ```Object.entries()```
- Creates an array which contains arrays of key/value pairs of an object. 

```
const user1 = {
  age: 26,
  mobile: 8801967402131,
  name: "Talha"
}
const user = Object.entries(user1);
console.log(user) 
//[["age", 26], ["mobile", 8801967402131], ["name", "Talha"]]
```
##### ```Object.assign()```
- Similar to the spread operator. Allows for objects to be combined together.

```
const user1 = {
  birthYear: 1988,
  name: "Jordan"
}
const user1NewVal = {
  age: 33,
}
const combineObj = Object.assign(user1, user1NewVal)
console.log(combineObj)
//
{
  age: 26,
  birtYear: 1993,
  name: "Talha"
}
```


## Question 12
Explain how JSON can be manipulated in JavaScript, using examples from the JavaScript programming language

JSON stands for JavaScript Object Notation. "JSON is a text-based data-interchange format used to exchange data between a server and a client" (tutorial republic). The benefit to using JSON is that it follows basic document structure that is both easy to use and read by both humans and computers. Even though we'd expect JSON to only work with the object data type as represented by its name, JSON also works with Arrays as they are a special form of objects.

Example of a JSON ```Object```:
```js
  {
    "book": {
        "title": "In Search of Lost Time",
        "author": "Marcel Proust",
        "year": 1913,
        "bestseller": true
    }
}
``` 

While JSON objects looks similar to JavaScript, they have syntactical and operational differences. JSON Objects can not include keys or values without double ticks (""), and analyse (a string or text) into logical syntactic components.

Example of a JSON ```array```:
```js
{
    "fruits": [
        "Orange",
        "Mango",
        "Grapefruit",
        "Pineapple"
    ]
}
```

##### JSON.stringify()

```JSON.stringify()``` is a method that turns JavaScript objects into a JSON string.

```
console.log(JSON.stringify({ color: "blue", available: true }));
// expected output: "{ "color": "blue", "available": true }"

console.log(JSON.stringify([new Number(3), new String('false'), new Boolean(false)]));
// expected output: "[3,"false",false]"

```

##### JSON.parse
The majority of JavaScript developers interact with JSON objects and documents when working with databases and or REST/WEB API's. ```JSON.parse``` can take a single parameter which is the JSON string to be converted into, and evaluated as a JSON object.

````
const car = '{"make": "Toyota", "model": "LandCruiser", "available": true }'
const object = JSON.parse(car);

console.log(obj.make);
console.log(obj.available);
````

The code above is passing a JSON string, ```car``` as a parameter to the ```JSON.parse()```. This allows the program access to the flat JSON string and return values in the string.

This will print ```Toyota``` and ```true``` to the console.


## Question 13
*For the code snippet provided below, write comments for each line of code to explain its functionality. In your comments you must demonstrates your ability to recognize and identify functions, ranges and classes*


```js

// Write notes

class Car { //declares and creates a new Car class object
  constructor(brand) { // creates and initializes objects created inside the class
    this.carname = brand; //a carname object is created by the constructor function and attributed to the brand variable/instance
  }
  present() { //this is considered an instance function as it extracts and returns data from the class object. The present function is called on the distance of an object.
    return 'I have a ' + this.carname; //the function returns and concatenates the string 'I have a ' with the brand instance.
  }
}

class Model extends Car { //creates a Model class object that inherits from Car class, inheriting the functions of the Car class
  constructor(brand, mod) { //like above, this method is creating and initializing object; it expects two parameters brand and mod
    super(brand); //Super is a key word used to access and call functions from Car parent class
    this.model = mod;//like in the car class, the program will create a model object and initialize it
  }
  show() {//the show function is also initialized
    return this.present() + ', it was made in ' + this.model; // The show function is calling the present function from the Car parent class, using string concatenation and joining the return statement to an instance of model
  }
}

let makes = ["Ford", "Holden", "Toyota"] //assigns an array of elements and assigns it to makes
let models = Array.from(new Array(40), (x,i) => i + 1980) //the models variable is given the value of Array.from(), or a static copied array object, of 40 elements. The elements start at the number 1980 and increment by 1, or i which is the iterator. 


function randomIntFromInterval(min,max) { // declaring a function with two parameters.
    return Math.floor(Math.random()*(max-min+1)+min);
} // Math.random() returns a floating-point number greater than or equal to 0, and less than 1.
  // the difference of max and min added by 1 plus the min number is then multiplied by the random floating point number returned by Math.random
  // it is then rounded down to the nearest whole number using the Math.floor method and returned
  
}

for (model of models) { //the for loop is iterating through each element in the models array

  make = makes[randomIntFromInterval(0,makes.length-1)]// the make variable being assigned the value of an element from the makes array, selected by targeting its index in bracket notation. The index is found by calling the randomIntFromInterval function and selecting a random index number within the limits of the length of the array. 0 being the min parameter and makes.length-1 being the max parameter.
  model = models[randomIntFromInterval(0,makes.length-1)]// the same function called on the models array and assigned to the model variable

  mycar = new Model(make, model);// assigns a new instance of the Model Class with make and model varibales as the parameters 
  console.log(mycar.show())// the show function is called on the instance of the Model class saved to the mycar variable, returning a string.
}
```

This above function will print the string where the Make and year of car are chosen at random.

```I have a Ford, it was made in 1988```
```I have a Toyota, it was made in 1993```















