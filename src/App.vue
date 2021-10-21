<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/layout/Header.vue";
import Search from "./components/Search.vue";
import Slider from "./components/slider/index.vue";
import Slide from "./components/slider/Slide.vue"
</script>

<template>
  <Header />
  <div class="container">
    <Search />
    <Slider class="pt-3">
      <Slide></Slide>
      </Slider>
  </div>
  <!-- <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite" /> -->
</template>

<style lang="scss">
@import "./assets/scss/index.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
