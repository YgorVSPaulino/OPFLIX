<script>
 export default {
  
  methods:{
    goToHome() {this.$router.push('/')} 
  }
}
</script>

<template>
  <main class="bg-main">
    <!-- Componente Nav -->
    <header class="p-4 bg-black">
    <div class="container mx-auto flex justify-between items-center">
      <img src="../assets/imgs/Logo.png" alt="" width="150px" @click="goToHome">
    </div>
  </header>
    <!-- Conteúdo do HomeView -->
    <div class="flex justify-center items-center p-20">
      <div class="w-full max-w-md">
        <div
          class="flex flex-col items-center justify-center">
          <h1 class="text-6xl font-bold mb-4">Lost your way?</h1>
          <h4 class="text-3xl text-black mb-8 text-center">
            Sorry, we can’t find that page. You’ll find lots to explore on the home page.
          </h4>
          <router-link
            to="/"
            class="bg-black text-white font-bold py-2 px-6 rounded hover:bg-gray-800 transition-colors">
            OPFLIX Home
          </router-link>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.bg-main {
  background-image: url("../assets/imgs/bgerror.png");
  background-size: cover;
  background-position: center;
  height: 100vh;
  /* para cobrir a tela toda */
}
</style>
