<template>
  <div>I'm a parent block!!!</div>

  <div class="box a">AAA</div>
  <div class="box b">BBB</div>
  <div class="box c">CCC</div>

  <ChildBlock />
</template>

<script setup lang="ts">
import ChildBlock from './ChildBlock.vue';
</script>

// Block Scoped
<style scoped>
.b {
  background: lime;
}

.c {
  background: cyan;
}
</style>

// Global style
<style>
.box {
  height: 100px;
  width: 100px;
  border: 5px dotted black;
}

.a {
  background: red;
}
</style>
