<template>
  <Header/>
  <Separator/>
</template>

<script setup>
import Header from './components/Header.vue';
import Separator from "./components/Separator.vue";

</script>

<style>

@import './styles/quick-flex.css';
@import './styles/reset.css';

@font-face {
  font-family: "Futura";
  src: url("./assets/futura/futur.ttf") format('truetype');
}


@font-face {
  font-family: "Futura Italics";
  src: url("./assets/futura/Futura Bold Italic font.ttf") format('truetype');
}

#app {
  font-family: Futura, Avenir, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
}
</style>
