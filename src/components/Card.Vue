<script>

import Bottone from "./partials/Bottone.vue";

export default {

  name: "Card",

  components: {
    Bottone
  },

  props: {
    name: String,
    price: String,
  }
}


</script>


<template>
  <div class="flex p-5">
    <div class=" w-1/2 m-auto bg-blue-600 p-4 rounded-lg shadow-lg">
      <div class="flex justify-between pb-4">
        <p class="text-white font-bold text-5xl">{{ name }}</p> <!-- Passato con props -->
        <h1 class="text-white text-3xl py-3">Slot</h1>
      </div>
      <div class="p-5 bg-white rounded">
        <slot>
        </slot>

        <div class="bg-blue-500 h-100"></div>

        <div class="flex justify-between">
          <h1 class="py-3 font-bold">Prezzo : {{ price }} euro</h1>
          <div class="flex gap-5">
            <Bottone functionality="Acquista" bgColor="bg-green-600" />
            <Bottone functionality="Elimina" bgColor="bg-red-600" />
          </div>
        </div>
      </div>

    </div>
  </div>


</template>

<style>

</style>