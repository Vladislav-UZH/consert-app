<script setup>
import TheCard from "./components/TheCard.vue";

const cards = 200;
</script>

<template>
  <div>
    <header>
      <span>UZHNU</span>
      <span>БЛАГОДІЙНИЙ КОНЦЕРТ - ЛОТЕРЕЯ</span>
      <span>UZHNU</span>
    </header>
  </div>
  <ul class="list">
    <li v-for="(item, index) in cards" :key="index">
      <TheCard :number="index + 1" />
    </li>
  </ul>
</template>

<style scoped>
.list {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
}
</style>
