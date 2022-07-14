<script setup>
import { ref } from 'vue';
import Upvote from './Upvote.vue';
const counts = ref(0);
</script>

<template>
  <div class="row">
    <div class="row-wrapper">
      <div v-if="counts > 0" class="row vote">
        <li v-for="count in counts"><Upvote /></li>
      </div>
    </div>
    <span v-if="counts < 7" class="button">
      <img src="../assets/add.svg" alt="arrow" @click="counts++" />
    </span>
  </div>
</template>

<style scoped>
.row {
  display: flex;
  list-style: none;
  flex-direction: row;
}
.row-wrapper {
  border: 1px solid lightgray;
  border-radius: 10px;
  width: 260px;
}
.vote {
  align-items: start;
  padding: 1px;
  margin: 3px;
  border-radius: 5px;
}
.button {
  align-items: end;
  height: 28px;
  width: 28px;
  padding: 2px;
  margin: 10px;
  border-radius: 7px;
  background: #f4f6f8;
  color: #343a40;
}
.button:hover {
  cursor: pointer;
}
</style>
