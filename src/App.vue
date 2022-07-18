<template>
  <div id="app">
    <h1>
      {{ $options.myTitle }}
    </h1>
    <h3 class="np-credits">
      {{ $options.myDescripion }}
    </h3>
  </div>
</template>

<script>
import { myTitle, myDescripion } from "./constants";

export default {
  name: "App",
  created() {
    this.$options.myTitle = myTitle;
    this.$options.myDescripion = myDescripion;
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding: 24px;
}
</style>