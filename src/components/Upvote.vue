<script setup>
import arrow from '../assets/arrow.svg';
</script>
<template>
  <div class="vote normal"><img :src="arrow" alt="arrow" /></div>
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
.selected {
  background: #e5e8fd;
  color: #253cf2;
}
.normal {
  background: #f4f6f8;
  color: #343a40;
}
</style>
