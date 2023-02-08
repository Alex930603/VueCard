<template>

  <button :class="{
    [bgColor]: true,        /* Quando viene dato un valore alla props bgColor, quello verrà inserito nella classe tailwind del bottone */
    [fontColor]: true,
    'text-white': !fontColor,
  }" class="font-bold py-2 px-10 rounded">{{ functionality }}
    <!-- props functionality value can be declared in other page,like this we can create differnt buttons easy -->

  </button>

</template>

<script>

export default {

  name: "Bottone",

  props: {
    functionality: String,
    bgColor: String,
    fontColor: String,
  }
}


</script>