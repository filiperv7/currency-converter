<template>
  <v-container>
    <nav-bar></nav-bar>

  <form>
    <section>
      <label for="test">1º Moeda</label>
      <v-row align="center">
        <v-col
          class="d-flex"
          cols="12"
          sm="6" id="test"
        >
          <v-select
            :items="items"
            label="Escolha a moeda"
          ></v-select>
        </v-col>
      </v-row>
    </section>

    <section>
      <label for="test2">2º Moeda</label>
      <v-row align="center">
        <v-col
          class="d-flex"
          cols="12"
          sm="6" id="test2"
        >
          <v-select
            :items="items"
            label="Escolha a moeda"
          ></v-select>
        </v-col>
      </v-row>
    </section>
  </form>

  </v-container>
</template>

<script>
import NavBar from '@/components/shared/NavBar.vue'

  export default {
    name: 'ConverterPage',
    components: { NavBar },
    data: () => {
      return {
        items: ['Dólar', 'Real', 'Rublo', 'Franco Suíço'],
      }
    },
  }
</script>

<style scoped>
  form {
    margin-top: 66px;

    display: flex;
    gap: .6rem;
  }

</style>