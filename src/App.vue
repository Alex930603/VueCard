<script setup>

import Card from "../components/Card.vue"

</script>

<template>

  <header>


  </header>

  <main>
    <div class="wrapper">
      <Card name="Props" price="34000"> <!-- Passato con props -->
        <!-- passate con slot -->
        <img class="py-5"
          src="http://www.casevenditapisa.it/wp-content/uploads/2020/02/vendita-piano-terra-di-villa-duplex-con-giardino-a-tirrenia-700x450.jpg" />
      </Card>

    </div>

  </main>
</template>

<style scoped>

</style>