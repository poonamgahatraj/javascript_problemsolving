<template></template>
<script>
let is_array=function(input){
  if(input instanceof Array)
    {
      return true;
    }
  else {
    return false;
  }
}

console.log(is_array("hello"))
console.log(is_array([1,2,3]))

//cloning an array

let array=[1,2,3,4]
let clone_array=[]
// clone_array=array
// console.log(array);
// console.log(clone_array)

//loop method
//  for(let i=0; i<=array.length;i++){
//     clone_array=array
//  }

//  console.log(array);
//  console.log(clone_array)

 clone_array=array.slice();
 console.log(array);
 console.log(clone_array)


 //simple JavaScript program to join all elements of the following array into a string

//  let arr =["hello","this","is","Poonam"]

//  console.log(arr.join(""))
//  console.log(arr.toString())


 //Write a JavaScript program to find the most frequent item in an array.

 let arr = [ 
    1, 1, 3, 5, 7, 6, 8, 5, 6, 4, 
    7, 6, 0, 2, 1, 6, 8, 9, 5, 
]; 
  
arr.sort((a, b) => a - b); 

console.log(arr) ;

let count=1;
let max=0;
let el;

for(let i=1;i<=arr.length;i++)
  {
    if(arr[i]===arr[i-1]){
      count++
    }
    
    else {
      count=1
    }
    
    if(count>max){
      max=count;
      el = arr[i];
    }
  
  }
console.log(el);

//Write a JavaScript program to sort the items of an array.
let arr1= [ -3, 8, 7, 6, 5, -4, 3, 2, 1 ];

arr1.sort((a,b)=>(a-b))

console.log(arr1)

//Write a JavaScript program that accepts a string as input and swaps the case of each character.

const str = "The Quick Brown Fox";

const result = str
  .split("")
  .map(item => (item === item.toUpperCase() ? item.toLowerCase() : item.toUpperCase()))
  .join("");

console.log(result);

//JavaScript program to find the sum of squares of a numerical vector.
let arr2=[1,2,3,4]
let sum=0;

for (let i=0;i<arr2.length;i++){
  sum+=Math.pow(arr2[i],2);
  
}
console.log(sum)


// JavaScript program to compute the sum and product of an array of integers.

let arr3=[1,2,3,4,5]
let sum1=0;
let product=1;

for(let i=0;i<arr3.length;i++)
{
  sum1+=arr3[i]
  product*=arr3[i]
}

console.log(sum1);
console.log(product);

//a JavaScript program to shuffle an array.

const arr4 = ['1','2','3','4','5','6','7','8','9'];


const shuffledArr = arr4.sort(() => Math.random() - 0.5);
console.log(shuffledArr);

// JavaScript program to compute the sum of each individual index value in the given array.

var array1 = [16,0,2,3,4]
var array2 = [3,5,6,7,8,13]
var l = Math.max(array1.length, array2.length);
var result1 = Array(l);
for(var i=0; i<l; ++i) result1[i] = (array1[i] || 0) + (array2[i] || 0);

console.log(result1)

//Write a JavaScript program to find duplicate values in a JavaScript array.

let check_duplicate_in_array = (input_array) => {
    input_array = input_array.sort((a, b) => a - b);
    let duplicate_elements = []
    for (let i=1; i<=input_array.length;i++) 
    {
        if (input_array[i] ===
            input_array[i - 1]) {
            duplicate_elements.push(
                input_array[i]);
        }
    }
   return [...new Set(duplicate_elements)];
}
let array3 = [1,2,3,4,2,1,3];
console.log(check_duplicate_in_array(array3));

</script>