<template>
    <header class="p-4">
    <div class="container mx-auto flex justify-between items-center">
      <img src="../assets/imgs/Logo.png" alt="" width="150px" @click="goToHome">
      <nav class="bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded">
        <RouterLink to="/login">Login</RouterLink>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  
  methods:{
    goToHome() {this.$router.push('/')} 
  }
}
</script>
<!-- methods: {
  // Defina o método para redirecionar para a rota /home
  goToHome() {
    this.$router.push('/home');
  }
} -->