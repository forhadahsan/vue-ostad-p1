<script setup>
import  data  from "./data/data"
const number = 12
const part6Title = "This is <b> Bold </b> Part 6 of the <strong> Vue.js App </strong> "

const url = "https://www.pexels.com/search/"
const animal = "cat"

const go = {
  title: "Welcome to My Portfolio",
  description: "This is a simple portfolio page built with Vue.js and Tailwind CSS.",
  image: "https://images.unsplash.com/photo-1506765515384-028b60a970df",
  buttonText: "Learn More",
}



</script>

<template>
  <div>
    <h2 class="text-4xl font-bold mb-6"> Part 6</h2>
    <p v-html="part6Title" class="text-2xl mb-4"> 
       
    </p>
  </div>
  <div>
    <h2 class="text-4xl font-bold mb-6">
      PArt 5
    </h2>
    <h3> 
      <a :href="url+animal" target="_blank" >Search For {{ animal }} </a>  
    </h3>
  </div>
<div>
  <h1 class="text-4xl font-bold mb-6"> Part 4 </h1>
  <h2 class="text-3xl font-bold mb-3"> Javascript Expression & calculation </h2>
  <h4 class="mb-2"> {{ number }} / 4 = <b>  {{  number / 4 }} </b> </h4>
  <h4 class="mb-2"> {{ number }} * 4 = <b>  {{  number * 4 }} </b></h4>
  <h4 class="mb-2"> {{ number }} + 4 = <b>  {{  number + 4 }} </b> </h4>
  <h4 class="mb-2"> {{ number }} - 4 = <b>  {{  number - 4 }} </b> </h4>
  <h4 class="mb-2"> {{ number }} % 4 = <b>  {{  number % 4 }} </b></h4>
  <h4 class="mb-2"> {{ number }} ** 4 = <b> {{  number ** 4 }}</b>  </h4>
  <h4 class="mb-2"> {{ number }} ** 2 = <b> {{  number % 2 == 0 ? "Even" : "Odd" }}</b>  </h4>
</div>




  <section class="flex flex-col items-center text-center bg-gray-100 p-10 rounded-xl shadow-lg">
    <h2 class="text-3xl font-bold mb-6"> Part 3 </h2>
    <h2 class="text-3xl font-bold mb-6"> {{  go.title }} </h2>
  <img :src="go.image" :title="go.title" alt="A cool visual" class="w-full max-w-md rounded-2xl mb-6 shadow-md">
  <p>{{ go.description }}</p>
   <a :href="go.image" :alt="go.title" :title="go.title" class="bg-gray-400 p-2 rounded" > View Image</a>
</section>

  <!-- part 2 -->
  <section class="flex flex-col items-center text-center bg-gray-100 p-10 rounded-xl shadow-lg">
    <h2 class="text-3xl font-bold mb-6"> Part 2 </h2>
    <h2 class="text-3xl font-bold mb-6"> {{  go.title }} </h2>
  <img :src="go.image" :title="go.title" alt="A cool visual" class="w-full max-w-md rounded-2xl mb-6 shadow-md">
  <p>{{ go.description }}</p>
  <button class="bg-red-800 text-black px-6 py-3 rounded-xl text-lg hover:bg-blue-700 transition">
    {{  go.buttonText }}
  </button>
</section>

 
<!-- part 1 -->
  <div class="bg-blue-500 text-white p-4 rounded-lg mt-2">
    <h2 class="text-3xl font-bold mb-6"> Part 1 </h2>
    <h3 class="ob"> It's Object declear</h3>
    <p> {{  data.name }} </p>
    <p> {{  data.age }} </p> 
    <h4> You have Total {{  data.tasks.length }} Task today</h4>
  </div>
</template>

<style scoped>
 .ob{
  color: rgb(224, 173, 31);
  font-family: 'Courier New', Courier, monospace; 
 }
</style>
