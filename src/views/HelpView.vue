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
        <div class="flex bg-white opacity-80 p-11 shadow-lg rounded-lg flex-col space-y-6">
  <h1 class="text-2xl text-black">
    Atualizar senha, e-mail ou número de telefone
  </h1>

  <p>Como você prefere redefinir sua senha?</p>

  <form class="space-y-3">
    <label class="flex items-center space-x-2">
      <input type="radio" name="group1" value="option1" />
      <span>Email</span>
    </label>

    <label class="flex items-center space-x-2">
      <input type="radio" name="group1" value="option2" />
      <span>Mensagem de Texto</span>
    </label>
  </form>

  <p>Enviaremos um email com instruções de como redefinir sua senha.</p>

  <input
    type="text"
    placeholder="Digite seu email"
    class="w-full max-w-md p-2 border bg-gray-400 border-gray-300 rounded-lg"
  />

  <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-lg w-full max-w-md">
    Enviar por email
  </button>
</div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.bg-main {
  background-image: url("../assets/imgs/Luffy.png");
  background-size: cover;
  background-position: center;
  height: 100vh;
  /* para cobrir a tela toda */
}
</style>
