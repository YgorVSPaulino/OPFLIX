<script setup>
/* import Nav from './components/Nav.vue'; */
</script>

<template>
  <header class="p-4">
    <div class="container mx-auto flex justify-between items-center">
      <img src="./assets/imgs/logo.png" alt="" width="150px">
      <nav>
        <RouterLink to="/login">Login</RouterLink>
      </nav>
    </div>
  </header>
  <RouterLink></RouterLink>
</template>

<style scoped>

</style>