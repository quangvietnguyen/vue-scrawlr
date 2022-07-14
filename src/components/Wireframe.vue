<script setup>
import { ref } from 'vue';
import Row from './Row.vue';
import { createStore } from 'vuex';
const store = createStore({
  state: {
    filled: false,
  },
  mutations: {
    change(state) {
      state.filled = !state.filled;
    },
  },
});
const counts = ref(0);
</script>

<template>
  <div class="card">
    <li v-for="row in 3"><Row /></li>
  </div>
</template>

<style scoped></style>
