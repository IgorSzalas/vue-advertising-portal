<script setup lang="ts">
import { RouterLink } from 'vue-router'

interface loginData {
  email: string | undefined | null
  password: string | undefined | null
}

let loginData: loginData = {
  email: '',
  password: ''
}
</script>

<template>
  <div id="login">
    <div id="login-form">
      <input
        class="login-data"
        placeholder="E-mail"
        type="text"
        :value="loginData.email"
        @input="(event) => (loginData.email = event.target.value)"
      />
      <input
        class="login-data"
        placeholder="Hasło"
        type="text"
        :value="loginData.password"
        @input="(event) => (loginData.password = event.target.value)"
      />
      <RouterLink id="register" to="/register">Nie masz konta? Zarejestruj się!</RouterLink>
      <button id="login-button" @click="">Zaloguj się</button>
    </div>
  </div>
</template>

<style scoped>
#register {
  text-decoration: none;
}

#login {
  display: flex;
  justify-content: center;
  align-items: center;
}

#login-form > * {
  margin: 1rem;
}

#login-form {
  display: flex;
  flex-direction: column;
}

#login-button {
  padding: 0.5rem;
}

.login-data {
  padding: 0.5rem;
}
</style>
