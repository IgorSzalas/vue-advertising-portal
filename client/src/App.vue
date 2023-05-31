<script setup lang="ts">
import Navbar from './components/Navbar.vue'
import { RouterView } from 'vue-router'
</script>

<template><Navbar /><RouterView /></template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
