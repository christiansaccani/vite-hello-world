<script >

  import AppTitle from "./components/AppTitle.vue";
  import AppHero from "./components/AppHero.vue";

  export default {
  components: {
    AppTitle,
    AppHero,
  }
}

</script>

<template>

  <div id="container">
    <AppTitle></AppTitle>
    <AppHero></AppHero>
  </div>

</template>

<style >

  #container {
    margin: 20px;
  }

</style>
