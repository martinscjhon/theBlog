<template>
  <div id="app">
    <HeaderComponent />
    <HomeComponent />
    <AboutUsComponent />
    <CategoryComponent />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/Header.vue';
import HomeComponent from './components/Home.vue';
import AboutUsComponent from './components/AboutUs.vue';
import CategoryComponent from './components/Category.vue';
import FooterComponent from './components/Footer.vue';

export default {

  name: 'App',
  components: {
    HeaderComponent,
    HomeComponent,
    AboutUsComponent,
    CategoryComponent,
    FooterComponent,
  },
};
</script>

<style>

</style>
