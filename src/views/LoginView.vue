<script>
export default {
  
  methods:{
    goToHome() {this.$router.push('/')} 
  }
}
</script>

<template>
  <main class="bg-main">
    <!-- Componente Nav incluído no HomeView -->
    <header class="p-4">
    <div class="container mx-auto flex justify-between items-center">
      <img src="../assets/imgs/Logo.png" alt="" width="150px" @click="goToHome">
    </div>
  </header>
    <!-- Conteúdo do HomeView -->
    <div class="flex justify-center items-center">
      <div class="w-full max-w-md">
        <div class="bg-black opacity-90 p-11 shadow-lg rounded-lg">
          <h2 class="text-2xl font-bold text-center mb-6 text-white">Entrar</h2>

          <form @submit.prevent="submitLogin">
    <!-- Campo de Email com label dentro do input -->
    <div class="mb-6 relative">
      <input
        v-model="email"
        id="email"
        type="email"
        placeholder=" "
        class="bg-gray-700 text-white w-full p-4 pt-6 rounded border border-gray-500 focus:outline-none focus:border-blue-500 peer"
        required
      />
      <label
        for="email"
        class="absolute text-gray-400 left-4 top-4 transform scale-100 origin-[0] transition-all duration-200 ease-in-out peer-placeholder-shown:top-4 peer-placeholder-shown:left-4 peer-placeholder-shown:scale-100 peer-focus:top-1 peer-focus:left-4 peer-focus:scale-75 peer-focus:text-blue-500"
      >
        Email ou numero de celular
      </label>
    </div>

    <!-- Campo de Senha com label dentro do input -->
    <div class="mb-6 relative">
      <input
        v-model="password"
        id="password"
        type="password"
        placeholder=" "
        class="bg-gray-700 text-white w-full p-4 pt-6 rounded border border-gray-500 focus:outline-none focus:border-blue-500 peer"
        required
      />
      <label
        for="password"
        class="absolute text-gray-400 left-4 top-4 transform scale-100 origin-[0] transition-all duration-200 ease-in-out peer-placeholder-shown:top-4 peer-placeholder-shown:left-4 peer-placeholder-shown:scale-100 peer-focus:top-1 peer-focus:left-4 peer-focus:scale-75 peer-focus:text-blue-500"
      >
        Senha
      </label>
    </div>

    <!-- Botões Entrar e Código de Acesso -->
    <div class="flex flex-col space-y-4">
      <button type="submit" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded w-full">
        Entrar
      </button>

      <div class="text-center text-gray-400">OU</div>

      <button type="button" class="bg-gray-500 hover:bg-gray-700 text-white font-bold py-2 px-4 rounded w-full">
        Código de Acesso
      </button>
    </div>

    <!-- Link de recuperação de senha -->
    <router-link to="/help" class="block text-center mt-6 text-sm text-blue-500 hover:text-blue-700">
      Esqueceu sua senha?
    </router-link>
  </form>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.bg-main {
  background-image: url("../assets/imgs/background2.png");
  background-size: cover;
  background-position: center;
  height: 100vh; /* para cobrir a tela toda */
}
input:focus ~ label,
input:not(:placeholder-shown) ~ label {
  transform: translateY(-1.5rem) scale(0.75);
}

label {
  background-color: transparent;
  padding: 0 0.25rem; /* Opcional: Espaço para não colidir com a borda do input */
}
</style>
