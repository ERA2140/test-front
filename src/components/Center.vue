

<template >
  <hr class="mt-10">
  <h2 >Second test: </h2>
  <p>
    1 Display this text as a proper ordered list
    2 Center the orange rectangle vertically and horizontally in its parent
    3 Center the text inside the orange square vertically and horizontally
    4 Set the text "center me" in capital with the 1st letter in white without adding extra tag, css class to the div or p tag
    5 In mobile view (800px), the orange rectangle should be green
    6 Transform the orange rectangle to a losange but keep the text inside horizontal
    7 Complete the code so when we click on the orange rectangle it should follow the mouse cursor on the screen
  </p>
  <div>{{positionX}} {{positionY}}</div>
  <div class="parent">
    <div class="child" :style="{ top:positionY + 'px', left:positionX + 'px' }"><p>center me!</p></div>
  </div>

</template>
<script setup lang="ts">
import {onMounted, ref} from 'vue'

const positionX = ref(0)
const positionY = ref(0)

onMounted(()=> {
  document.addEventListener('mousemove', update)

})

function update(e) {
  positionX.value = e.clientX
  positionY.value = e.clientY
}

</script>
<style >
.parent{
  background-color: lightsteelblue;
  width: 100%;
  height: 500px;
}
.child {
  width: 200px;
  height: 150px;
  background-color: orangered;
}
</style>
