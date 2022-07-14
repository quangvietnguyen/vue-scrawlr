<script setup>
import arrow from '../assets/arrow.svg';
</script>
<script>
export default {
  props: ['store'],
};
const selected = { background: '#e5e8fd', color: '#253cf2' };
const normal = { background: '#f4f6f8', color: '#343a40' };
</script>
<template>
  <div class="vote" :style="[store.state.filled ? selected : normal]">
    <img :src="arrow" alt="arrow" @click="store.commit('change')" />
  </div>
</template>
<style scoped>
.vote {
  height: 28px;
  width: 28px;
  padding: auto;
  margin: 1px;
  border-radius: 5px;
}
.vote:hover {
  cursor: pointer;
}
</style>
