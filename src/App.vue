<template>
  <div id="app">
    <HeaderComponent />
    <HomeComponent />
    <AboutUsComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue';
import HomeComponent from './components/Home.vue';
import AboutUsComponent from './components/AboutUs.vue';

export default {

  name: 'App',
  components: {
    HeaderComponent,
    HomeComponent,
    AboutUsComponent,
  },
};
</script>

<style>

</style>
