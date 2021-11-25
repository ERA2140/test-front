<template>
    <h2>First test: </h2>
    <p>Write a function that prints all the numbers from 1 to 100 when you click on the button FIZZBUZZ”.<br>
      But for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”.
      For numbers which are multiples of both three and five print “FizzBuzz”.<br>
      The add button will do the same thing but step by step for exemple if we click 3 time on it after reset the content we will have : 1,2,Fizz<br>
      your code should pass the FizzBuzz e2e test you can test it by running ( yarn abracadabra or npm run abracadabra)
    </p>
    <div class="flex gap-1 justify-center">
      <button id="addBtn" class="p-2 rounded text-white bg-blue-600 hover:bg-blue-900"   type="button" @click="addAction">ADD</button>
      <button id="fizzbuzzBtn" class="p-2 rounded text-white bg-blue-600 hover:bg-blue-900"  type="button" @click="fizzbuzzAction" >FIZZBUZZ</button>
      <button id="resetBtn" class="p-2 rounded text-white bg-red-600 hover:bg-red-900"  type="button" @click="resetAction">RESET</button>
    </div>
    <div id="content" class="p-2 m-2 rounded bg-green-800  break-words  text-white">{{ getText() }}</div>

</template>
<script setup lang='ts'>
import {  ref } from "vue"

const output = ref(Array<string>());

function addAction (){
}

function resetAction(){
}

function fizzbuzzAction(){
}

function getText(){
    return output.value.join(',')
}

</script>
