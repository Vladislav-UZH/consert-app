<script setup>
import { reactive } from "vue";

defineProps({
  number: Number,
});

const data = reactive({
  owner: "John Stone",
});
</script>

<template>
  <div class="card">
    <span class="card-text">CARD-{{ number }}</span>
  </div>
</template>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* width: 100%; */
  width: 224px;
  padding: 24px 80px;

  border: var(--border);
  background-color: var(--base);
  border-radius: 15px;
}
.card-text {
  font-size: 32px;
}
</style>
