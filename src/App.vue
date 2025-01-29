<template>
  <navBar />
  <div class="container flex my-5 g-4">
    <firstCard />

    <secondCard />

    <thirdCard />

    <fourthCard />

    <fifthCard />

    <sixthCard />
  </div>

  <footerCard />
</template>

<script lang="js" setup>
import navBar from './components/mainComps/navBar.vue'
import firstCard from './components/Cards/firstCard.vue'
import secondCard from './components/Cards/secondCard.vue'
import thirdCard from './components/Cards/thirdCard.vue'
import fourthCard from './components/Cards/fourthCard.vue'
import fifthCard from './components/Cards/fifthCard.vue'
import sixthCard from './components/Cards/sixthCard.vue'
import footerCard from './components/Cards/footerCard.vue'
</script>
