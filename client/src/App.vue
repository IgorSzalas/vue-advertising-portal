<script setup lang="ts">
import Navbar from './components/Navbar.vue'
import { RouterView } from 'vue-router'
import { provide } from 'vue'

const dummmyCategoriesData: categoriesData[] = [
  {
    id: 1,
    categoriesTitle: 'Samochody',
    categoriesDescription: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur molestiae rerum
      architecto quae. Incidunt sequi necessitatibus dignissimos. Reprehenderit omnis ipsam minima
      temporibus sit dicta magni, hic veritatis aperiam saepe odio.`
  },
  {
    id: 2,
    categoriesTitle: 'Samochody',
    categoriesDescription: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur molestiae rerum
      architecto quae. Incidunt sequi necessitatibus dignissimos. Reprehenderit omnis ipsam minima
      temporibus sit dicta magni, hic veritatis aperiam saepe odio.`
  },
  {
    id: 3,
    categoriesTitle: 'Samochody',
    categoriesDescription: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur molestiae rerum
      architecto quae. Incidunt sequi necessitatibus dignissimos. Reprehenderit omnis ipsam minima
      temporibus sit dicta magni, hic veritatis aperiam saepe odio.`
  }
]

export interface categoriesData {
  id: number
  categoriesTitle: string
  categoriesDescription: string
}

const sendDummyCategoriesData = provide('data', dummmyCategoriesData)
</script>

<template>
  <Navbar />
  <RouterView />
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
