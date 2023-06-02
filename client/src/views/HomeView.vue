<script setup lang="ts">
import Category from '@/components/Category.vue'
</script>

<template>
  HomeView
  <div id="main-page">
    <div id="categories-container">
      <Category />
      <Category />
      <Category />
    </div>
  </div>
</template>

<style scoped>
#categories-container {
  display: flex;
  flex-direction: row;
}
</style>
