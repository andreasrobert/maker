<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue";
import Intro from "./components/Intro.vue";
import Details from "./components/Details.vue";
import Pricing from "./components/Pricing.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <!-- <HelloWorld msg="Hello Vue 3 + Vite" /> -->

  <Header />
  <Intro />
  <Details />
  <Pricing />
  <Footer />
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Manrope:wght@500;800&display=swap");

body,
html {
  margin: 0px;
  height: 100%;
}

#app {
  font-family: "Manrope", sans-serif;
  text-align: center;
  color: white;
  background-color: #080c20;
  margin: 0px;
  display: flex;
  align-items: center;
  flex-direction: column;
  overflow: hidden;
}

h1 {
  color: white;
}

.xBold {
  font-weight: 800;
  font-size: 3.1vw;
  /* line-height: ; */
}

.bold {
  font-weight: 800;
  font-size: 40px;
  /* line-height: ; */
}

.sBold {
  font-weight: 800;
  font-size: 32px;
  /* line-height: ; */
}

.xMedium {
  font-weight: 800;
  font-size: 18px;
  /* line-height: ; */
}

.medium {
  font-weight: 500;
  font-size: 1vw;
  color: #777f98;
  /* line-height: ; */
}

@media only screen and (max-width: 1200px) {
  .medium {
    font-size: 1.3vw;
  }
}
</style>
