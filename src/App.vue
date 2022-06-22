<template>
  <div id="app">
  <!-- digunakan untuk melakukan input user -->
  <input v-model="message" placeholder="edit me">
  <!-- tempat untuk menampilkan inputan user -->
  <p>Hallo {{ message }}</p>
  </div>
</template>

<script>

</script>

<style>
/* Style untuk website seperti font dll */
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
