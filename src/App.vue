<template>
  <app-contact-block/>
  <app-navbar/>
  <router-view/>
  <app-footer/>
</template>

<script>
import AppNavbar from './components/AppNavbar.vue';
import AppFooter from './components/AppFooter.vue';
import AppContactBlock from './components/AppContactBlock.vue';

export default {
  components: {
    AppNavbar,
    AppFooter,
    AppContactBlock
}
}


</script>
<style>
#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
