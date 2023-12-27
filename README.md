# ![Alt text](https://miro.medium.com/v2/resize:fit:720/format:webp/1*-JdXoCEA_G0mS6gpHvRR4Q.png)

**This Repository is created for Day 3 Task**

+ How to compare two JSON have the same properties without order?
  
    + `a. let obj1 = { name: "Person 1", age:5};
       b. let obj2 = { age:5, name: "Person 1"};`

  +     let obj1 = { name: "Person1" , age : 5};

        let obj2 = {age : 5 , name:"Person1"};

        let result = true;

        if(Object.keys(obj1).length == Object.keys(obj2).length){

        for(let key in obj1){

        if(obj1[key] == obj2[key]){

            continue;

        }

        else{

            flag = false;

            break;
        }
        }
        }

        else{
        result = false;
        }
        if(result == true){
        console.log("______________JSON Properties are Identical______________");
        }
        else{
        console.log("______________JSON Properties are Non-Identical______________");
        }


+ Use the rest countries API URL -> https://restcountries.com/v3.1/all and display all the country flags in the console.

+ Use the same rest countries and print all country names, regions, sub-region and populations.