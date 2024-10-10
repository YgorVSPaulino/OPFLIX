<script setup>
import Nav from '../components/Nav.vue';
</script>

<template>
  <main class="bg-main">
    <!-- Componente Nav incluído no HomeView -->
    <Nav></Nav>
    <!-- Conteúdo do HomeView -->
    <div class="text-center p-8 my-20">
      <div>
        <h1 class="text-white text-4xl font-bold">Episódios, notícias e novidades <br> sobre One Piece e muito <br> mais sem limites</h1>
        <h4 class="text-white text-xl font-semibold mt-4">A partir de 20,90. Cancele quando quiser.</h4>
        <p class="text-white mt-6">Quer assistir? Informe seu e-mail para obter ou reiniciar sua assinatura.</p>
      </div>
      <div class="my-9 space-x-4">
    <!-- Input com efeito vidro -->
    <input
      type="text"
      class="w-96 bg-white bg-opacity-20 backdrop-blur-md border border-white/30 text-white placeholder-white p-2 rounded-lg"
      placeholder="Email"
    />

    <!-- Botão vermelho -->
    <button class="bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded-lg">
      Vamos lá
    </button>
  </div>
    </div>
  </main>
</template>

<style scoped>
.bg-main {
  background-image: url('../assets/imgs/background2.png');
  background-size: cover;
  background-position: center;
  height: 100vh; /* para cobrir a tela toda */
}
</style>