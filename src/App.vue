
<template>
  <PointBackground style="position: fixed;left: 0;right: 0; z-index: -999;" />
  <div class="app">
    <div>
      <h1>Hello World</h1>
      <button type="button" @click="switchTheme">切换</button>
    </div>
  </div>
  <div style="position: fixed;bottom: 1rem; right: 1rem;">
    <a href="https://github.com/xiaohuohumax/PointBackground" target="_blank">
      Github
    </a>
  </div>
</template>
<script setup lang="ts">
import PointBackground from './components/PointBackground.vue';

function switchTheme() {
  document.documentElement.classList.toggle('dark')
}
</script>