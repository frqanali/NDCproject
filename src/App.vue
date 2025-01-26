<template>
  <navBar />
  <div class="container flex m-5">
    <firstCard />
  </div>
  <div class="container flex m-5">
    <secondCard />
  </div>
  <div class="container flex m-5"><thirdCard /></div>
  <div class="container flex m-5">
    <fourthCard />
  </div>
  <div class="container flex m-5">
    <fifthCard />
  </div>
</template>

<script lang="js" setup>
import navBar from './components/mainComps/navBar.vue'
import firstCard from './components/Cards/firstCard.vue'
import secondCard from './components/Cards/secondCard.vue'
import thirdCard from './components/Cards/thirdCard.vue'
import fourthCard from './components/Cards/fourthCard.vue'
import fifthCard from './components/Cards/fifthCard.vue'
</script>
