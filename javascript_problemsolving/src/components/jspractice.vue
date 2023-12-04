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

</script>