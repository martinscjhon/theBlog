<template>
  <div id="app">
    <HeaderComponent />
    <HomeComponent />
    <AboutUsComponent />
    <CategoryComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue';
import HomeComponent from './components/Home.vue';
import AboutUsComponent from './components/AboutUs.vue';
import CategoryComponent from './components/Category.vue';

export default {

  name: 'App',
  components: {
    HeaderComponent,
    HomeComponent,
    AboutUsComponent,
    CategoryComponent,
  },
};
</script>

<style>

</style>
