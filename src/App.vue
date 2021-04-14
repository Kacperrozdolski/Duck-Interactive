<template>
  <div class="marketing">
    <main-hero></main-hero>
    <main-about></main-about>
    <main-services></main-services>
    <main-work></main-work>
    <main-contact></main-contact>
  </div>
</template>

<script>
import MainHero from "./components/MainHero.vue";
import MainAbout from "./components/MainAbout.vue";
import MainServices from "./components/MainServices.vue";
import MainWork from "./components/MainWork.vue";
import MainContact from "./components/MainContact.vue";

export default {
  name: "App",
  components: { MainHero, MainAbout, MainServices, MainWork, MainContact },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;700&display=swap");
body {
  margin: 0 !important;
  font-family: Poppins;
}
.marketing {
  min-height: 100vh;
  display: flex;
  align-items: center;
  flex-direction: column;
}
</style>
