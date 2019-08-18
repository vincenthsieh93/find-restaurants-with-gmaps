<template>
  <div id="app">
    <GoogleMaps />
  </div>
</template>

<script>
import GoogleMaps from "./components/GoogleMaps.vue";

export default {
  name: "app",
  components: {
    GoogleMaps
  }
};
</script>

<style lang="scss">
@import url(assets/style/reset.css);

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  display: flex;
  height: 100%;
  color: #2c3e50;
}
</style>
