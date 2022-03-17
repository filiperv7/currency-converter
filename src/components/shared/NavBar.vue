<template>
  <v-container>
    <v-app-bar app>
      <figure>
      <img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/PjwhRE9DVFlQRSBzdmcgIFBVQkxJQyAnLS8vVzNDLy9EVEQgU1ZHIDEuMS8vRU4nICAnaHR0cDovL3d3dy53My5vcmcvR3JhcGhpY3MvU1ZHLzEuMS9EVEQvc3ZnMTEuZHRkJz48c3ZnIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDMyIDMyIiB2ZXJzaW9uPSIxLjEiIHZpZXdCb3g9IjAgMCAzMiAzMiIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayI+PGcgaWQ9IkxheWVyXzEiLz48ZyBpZD0iTGF5ZXJfMiI+PGc+PGxpbmUgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDAwMDAwIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS1taXRlcmxpbWl0PSIxMCIgc3Ryb2tlLXdpZHRoPSIyIiB4MT0iMTYiIHgyPSIxNiIgeTE9IjEwIiB5Mj0iMTIiLz48bGluZSBmaWxsPSJub25lIiBzdHJva2U9IiMwMDAwMDAiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBzdHJva2Utd2lkdGg9IjIiIHgxPSIxNiIgeDI9IjE2IiB5MT0iMjAiIHkyPSIyMiIvPjxwYXRoIGQ9IiAgICBNMTQsMjBoM2MxLjEsMCwyLTAuOSwyLTJzLTAuOS0yLTItMmgtMmMtMS4xLDAtMi0wLjktMi0yczAuOS0yLDItMmgzIiBmaWxsPSJub25lIiBzdHJva2U9IiMwMDAwMDAiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLW1pdGVybGltaXQ9IjEwIiBzdHJva2Utd2lkdGg9IjIiLz48cGF0aCBkPSIgICAgTTE2LDZjNS41LDAsMTAsNC41LDEwLDEwcy00LjUsMTAtMTAsMTBTNiwyMS41LDYsMTZ2LTMiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2UtbWl0ZXJsaW1pdD0iMTAiIHN0cm9rZS13aWR0aD0iMiIvPjxwb2x5bGluZSBmaWxsPSJub25lIiBwb2ludHM9IiAgICAxMCwxNyA2LDEzIDIsMTcgICAiIHN0cm9rZT0iIzAwMDAwMCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2UtbWl0ZXJsaW1pdD0iMTAiIHN0cm9rZS13aWR0aD0iMiIvPjxwYXRoIGQ9IiAgICBNMTYsMmM3LjcsMCwxNCw2LjMsMTQsMTRzLTYuMywxNC0xNCwxNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDAwMDAwIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS1taXRlcmxpbWl0PSIxMCIgc3Ryb2tlLXdpZHRoPSIyIi8+PC9nPjwvZz48L3N2Zz4=" alt="Logo do site: a logo é no formato circular, com meio circulo envolto a um uma ceta curvada e dentro dela um sifrão, símbolo que representa o dinheiro.">
      </figure>
      <h2 class="title">Currency Converter</h2>
    </v-app-bar>
  </v-container>
</template>

<script>
  export default {
    name: 'NavBar',
  }
</script>

<style scoped>
  * {
    margin: 0;
  }
  body {
    margin: 0;
  }

  div.home-page v-app-bar {
    display: flex;
    align-items: center;


    padding-left: .6rem;
    height: 80px;
  }

  figure {
    flex-grow: 2;

  }
  figure img {
    max-width: 3rem;

  }

  h2.title {
    flex-grow: 10;

    margin-left: -1.5rem;
  }
</style>