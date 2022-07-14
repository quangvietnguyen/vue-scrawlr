<script setup>
import Wireframe from './components/Wireframe.vue';
</script>

<template>
  <div>
    <h1>Quang Viet Nguyen</h1>
    <h2>Scrawlr Vue 3 Assessment</h2>
    <h3>Using Vite and Vue 3 with Vuex Store</h3>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <Wireframe />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
