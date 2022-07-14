<script setup>
import Row from './Row.vue';
</script>

<template>
  <div class="card">
    <li v-for="row in 3"><Row /></li>
  </div>
</template>

<style scoped>
.card {
  border: solid 1px lightgray;
  border-radius: 10px;
  list-style: none;
}
</style>
