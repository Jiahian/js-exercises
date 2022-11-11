<template>
  <h1 class="text-3xl">Question 1</h1>
</template>

<script>
// Qn: Write a function that takes two numbers and returns the maximum of the two. 

// Concepts: 
// - Creating a Function
// - Using operations
// - If-else shortform (Ternary operation)

//Ans: 
let number = max(3,4); //max(3,3)
console.log(number);

function max(a,b) {
  if (a>b) return a
  else return b
  // shortform: return (a>b)? a: b;
}
</script>