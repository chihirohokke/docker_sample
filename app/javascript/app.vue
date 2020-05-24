<template>
  <v-app id="app"> <!--divから変更-->
    <Header/> <!--追記-->
    <h1>This is app.vue</h1> <!--追記-->
    <p>{{ message }}</p>
    <Top/> <!--追記-->
  </v-app>
</template>

<script>
import Header from "./components/Header"; //追記
import Top from "./components/Top"; //追記

export default {
  data: function () {
    return {
      message: "Hello Vue!"
    }
  },
  components: {
    Header, //追記
    Top, //追記
  }
}
</script>

<style scoped>
p {
  font-size: 2em;
  text-align: center;
}
</style>
