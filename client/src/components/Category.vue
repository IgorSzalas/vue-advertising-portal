<script setup lang="ts">
import { inject } from 'vue'
import type { categoriesData } from '@/App.vue'
const testData: categoriesData[] = inject('data', 'Brak kategorii')
</script>

<template>
  <div class="categories" v-for="category in testData">
    <h4 class="categories-title">{{ category.categoriesTitle }}</h4>
    <p class="categories-description">
      {{ category.categoriesDescription }}
    </p>
  </div>
</template>

<style scoped>
.categories {
  width: 100px;
  border-style: solid;
  border-width: 1px;
  border-radius: 20px;
}

.categories > * {
  margin: 1rem;
}
</style>
