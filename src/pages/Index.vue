<template>
  <p class="flex  justify-center ">
    Recommended IDE setup:
    <a href="https://code.visualstudio.com/" class="bg-green-800 text-white" target="_blank">VSCode</a>
    +
    <a href="https://github.com/johnsoncodehk/volar"  class="bg-green-800 text-white" target="_blank">Volar</a>
  </p>
  <FizzbuzzVue></FizzbuzzVue>

  <Center></Center>

  <h2 >Integration test</h2>
  <p>
    Integrate demo.png and demo2.png in css & html blocks below.
  </p>

  <EthereumBalance></EthereumBalance>

  <div>
    <hr>
    <h2>last Test  </h2>
    <p>
      this app is in English we wants to have a system to translate it to french we hope you will have fun to do it    </p>
  </div>

  <Bonus></Bonus>
</template>
<script setup lang="ts">
import FizzbuzzVue from '@/components/Fizzbuzz.vue';
import EthereumBalance from "@/components/EthereumBalance.vue";
import Center from "@/components/Center.vue";
import Bonus from "@/components/Bonus.vue";

</script>
