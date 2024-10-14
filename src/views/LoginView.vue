<script setup>
import Nav from "../components/Nav.vue";
</script>

<template>
  <main class="bg-main">
    <!-- Componente Nav incluído no HomeView -->
    <Nav></Nav>
    <!-- Conteúdo do HomeView -->
    <div class="flex justify-center items-center">
    <div class="w-full max-w-md">
      <div class="bg-black opacity-80 p-11 shadow-lg rounded-lg">
        <h2 class="text-2xl font-bold text-center mb-6 text-white">Entrar</h2>

        <form @submit.prevent="submitLogin">
          <div class="mb-4">
            <label for="email" class="block text-gray-700 font-bold mb-2">Email</label>
            <input
              v-model="email"
              id="email"
              type="email"
              placeholder="Digite seu email"
              class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              required
            />
          </div>

          <div class="mb-6">
            <label for="password" class="block text-gray-700 font-bold mb-2">Senha</label>
            <input
              v-model="password"
              id="password"
              type="password"
              placeholder="Digite sua senha"
              class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              required
            />
          </div>

          <button type="submit" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded w-full">
            Entrar
          </button>

          <a href="#" class="block text-center mt-4 text-sm text-blue-500 hover:text-blue-700">Esqueceu sua senha?</a>
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
</style>
