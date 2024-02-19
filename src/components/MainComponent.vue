<script setup lang="ts">
import { ref } from 'vue'
const count = ref(0);
</script>

<template>
  <div class="main-container">
    <h3 @click="count++" @contextmenu.prevent="count=0">
      Test Counter {{ count }}
    </h3>
  </div>
</template>

<style scoped>
.main-container {
  user-select: none;
}
</style>
