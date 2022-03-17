<template>
  <v-container class="home-page">
    <nav-bar></nav-bar>
    <main> 
      <section class="center">
        <h1>O melhor Conversor de Moedas do mundo</h1>
        <h3>Várias opções de moedas de várias partes do mundo.</h3>
        <p>Simular cambio em tempo real</p>
        <router-link to="/converter"><button><v-btn class="ma-2" outlined color="indigo">Fazer Cambio</v-btn></button></router-link>
      </section>
    </main>

  </v-container>
</template>

<script>
import navBar from '@/components/shared/NavBar.vue'

  export default {
    name: 'HomePage',

    components: { navBar},
  }
</script>

<style scoped>
  main {
    height: 80vh;

  }
  
  section {
    display: flex;
    flex-direction: column;
    gap: 1rem;

    margin-top: 40px;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
  }

  p {
    margin-top: -.5rem;
  }
  button {
    margin-top: 2rem;
  }

</style>