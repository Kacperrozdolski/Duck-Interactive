<template>
  <div class="marketing">
    <main-hero></main-hero>
  </div>
</template>

<script>
import MainHero from "./components/MainHero.vue";
export default {
  name: "App",
  components: { MainHero },
};
</script>

<style lang="scss">
body {
  margin: 0 !important;
}
.marketing {
  min-height: 100vh;
  display: flex;
  align-items: center;
  flex-direction: column;
}
</style>
