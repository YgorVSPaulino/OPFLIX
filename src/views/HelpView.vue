<script setup>
import Nav from "../components/Nav.vue";
</script>

<template>
  <main class="bg-main">
    <!-- Componente Nav incluído no HomeView -->
    <Nav></Nav>
    <!-- Conteúdo do HomeView -->
    <div class="flex justify-center items-center p-20">
      <div class="w-full max-w-md">
        <div class="flex bg-white opacity-80 p-11 shadow-lg rounded-lg flex-col">
          <h1 class="text-2xl text-center mb-6 text-black">
            Atualizar senha, e-mail ou número de telefone
          </h1>
          <p>Como você prefere redefinir sua senha?</p>
          <form>
            <label>
              <input type="radio" name="group1" value="option1" />
              Email
            </label>
            <br>
            <label>
              <input type="radio" name="group1" value="option2" />
              Mensagem de Texto
            </label>

          </form>

          <p>Enviaremos um email com instruções de como</p>

          <input type="text">
          <button>Enviar por email</button>
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
