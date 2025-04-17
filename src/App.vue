<script setup>
import  data  from "./data/data"

const go = {
  title: "Welcome to My Portfolio",
  description: "This is a simple portfolio page built with Vue.js and Tailwind CSS.",
  image: "https://images.unsplash.com/photo-1506765515384-028b60a970df",
  buttonText: "Learn More",
}
</script>

<template>
  <section class="flex flex-col items-center text-center bg-gray-100 p-10 rounded-xl shadow-lg">
  <h2 class="text-3xl font-bold mb-6"> {{  go.title }} </h2>
  <img :src="go.image" :title="go.title" alt="A cool visual" class="w-full max-w-md rounded-2xl mb-6 shadow-md">
  <p>{{ go.description }}</p>
  <button class="bg-red-800 text-black px-6 py-3 rounded-xl text-lg hover:bg-blue-700 transition">
    {{  go.buttonText }}
  </button>
</section>

 

  <div class="bg-blue-500 text-white p-4 rounded-lg mt-2">
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
