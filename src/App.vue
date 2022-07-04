<template>
  <div id="app">
    <HeaderComponent />
    <HomeComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue';
import HomeComponent from './components/Home.vue';

export default {

  name: 'App',
  components: {
    HeaderComponent,
    HomeComponent,
  },
};
</script>

<style>

</style>
