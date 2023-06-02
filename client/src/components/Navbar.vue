<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <header id="navbar">
    <RouterLink to="/">
      <div
        id="page-logo"
        src="https://www.google.com/url?sa=i&url=https%3A%2F%2Frootblog.pl%2Fyoutube-nowe-logo%2F&psig=AOvVaw1NC2T0fbkbgsw3JxQRDTnm&ust=1685643243627000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCPCSlceUoP8CFQAAAAAdAAAAABAJ"
      ></div>
    </RouterLink>
    <nav id="links-container">
      <RouterLink class="links" to="/">Strona główna</RouterLink>
      <RouterLink class="links" to="/login">Zaloguj się</RouterLink>
    </nav>
  </header>
</template>

<style scoped>
#navbar {
  background-color: #464646;
  display: flex;
  justify-content: space-between;
  height: 50px;
}

#page-logo {
  height: 50px;
  width: 50px;
  background-color: red;
}

#links-container {
  display: inline;
  padding: 15px;
}

.links {
  display: inline;
  margin: 20px;
  text-decoration: none;
  color: #ffffff;
}

.links:hover {
  color: #9a9a9a;
}
</style>
