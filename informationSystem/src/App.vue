<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>

    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/Login">Login</RouterLink>
      </nav>
    </div>
  
  <RouterView />

  
</template>

<style scoped>

</style>
