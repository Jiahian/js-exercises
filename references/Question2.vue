<template>
  <h1 class="text-3xl">Question 2</h1>
</template>

<script>
// Qn: Using a for loop, combine all the words in the array into a string and print it out.
// Expected output: I know my for loops :)

// Concepts: 
// - array
// - for-loop

//Ans: 
let words = ["I", "know", "my", "for", "loops :)"];
let result = "";

for (let i = 0; i < words.length; i++) {
    result = result + " " + words[i];
}

console.log(result.trim());
</script>