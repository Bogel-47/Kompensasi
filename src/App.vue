<template>
  <div id="app">
    Your Name
    <!-- digunakan untuk melakukan input user -->
    <input v-model="value" placeholder="Input Nama Anda">
    <!-- tempat untuk menampilkan inputan user -->
    <p>{{inputted}}</p>
  </div>
</template>

<script>
// digunakan agar ketika user melakukan input maka akan langsung tampil data yang ada
export default {
  name: "App",
  data() {
    return {
      value: "",
      inputted: ""
    };
  },
  watch: {
    value(val) {
      this.inputted = `Hallo ${val}`;
    }
  }
};
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
