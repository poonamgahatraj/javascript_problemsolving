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

 let arr =["hello","this","is","Poonam"]

 console.log(arr.join(""))
 console.log(arr.toString())

</script>