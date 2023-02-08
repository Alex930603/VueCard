<template>

  <button :class="{
    [bgColor]: true,
    [fontColor]: true,
    'text-white': !fontColor,
  }" class="font-bold py-2 px-10 rounded">{{ functionality }}</button>

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