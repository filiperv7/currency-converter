<template>
  <v-container data-app>
    <nav-bar></nav-bar>
    <main>
      <h1>Conversor de Moedas</h1>
      <h4>Escolha as duas moedas desejadas</h4>
    </main>

    <v-form>
      <section>
        <label for="test">1º Moeda</label>
        <v-row align="center">
          <v-col
            class="d-flex"
            cols="12"
            sm="6" id="test"
          >
            <v-select v-model="selected1"
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
            <v-select v-model="selected2"
              :items="items"
              label="Escolha a moeda"
            ></v-select>
          </v-col>
        </v-row>
      </section>

      <v-btn center dark @click="converter()">
        Go
      </v-btn>


    </v-form> 


  </v-container>
</template>

<script>
import NavBar from '@/components/shared/NavBar.vue'

  export default {
    name: 'ConverterPage',
    components: { NavBar },
    data: () => ({
        items: ['Dólar', 'Real', 'Rublo', 'Franco Suíço'],


        selected1: '',
        selected2: '',
        apiResult: [],
        arroz: ''
    }),
    methods: {
      async   converter() {
        switch (this.selected1) {
          case 'Dólar':
            this.selected1 = 'USD';
            break;
          case 'Real':
            this.selected1 = 'BRL';
            break;
          case 'Rublo':
            this.selected1 = 'RUB';
            break;
          case 'Franco Suíço':
            this.selected1 = 'CHF';
            break;
        }

        switch (this.selected2) {
          case 'Dólar':
            this.selected2 = 'USD';
            break;
          case 'Real':
            this.selected2 = 'BRL';
            break;
          case 'Rublo':
            this.selected2 = 'RUB';
            break;
          case 'Franco Suíço':
            this.selected2 = 'CHF';
            break;
        }

        console.log(`this.apiResult.${this.selected1}${this.selected2}.name`)
      
        const promise = await fetch(`https://economia.awesomeapi.com.br/last/${this.selected1}-${this.selected2}`)
        .then(response => response.json())
        .then(json => {
          this.apiResult = json
        })

        console.log(promise)
      
      },

    },
  }

</script>

<style scoped>
  main {
    margin-top: 66px;

    margin-bottom: 3rem;

  }
  v-form {

    display: flex;
    gap: .6rem;
  }

</style>