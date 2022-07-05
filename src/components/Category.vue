<template>
  <div id="category">
    <section>
      <div v-for="category in category" :key="category.alt">
        <img :src="category.image" :alt="category.alt" />
        <p>{{category.data}}</p>
        <h3>{{category.title}}</h3>
        <p>{{category.text}}</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'CategoryComponent',
  data() {
    return {
      category: [
        {
          // eslint-disable-next-line global-require
          image: require('../assets/images/post-2.png'),
          alt: 'component-category-post-2',
          data: 'Janeiro 04, 2022',
          title: '10 dicas para conseguir a vaga desejada',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique.',
        },
        {
          // eslint-disable-next-line global-require
          image: require('../assets/images/post-3.png'),
          alt: 'component-category-post-3',
          data: 'Janeiro 04, 2022',
          title: 'Deixe seu código mais semântico com essas dicas',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique.',
        },
        {
          // eslint-disable-next-line global-require
          image: require('../assets/images/post-4.png'),
          alt: 'component-category-post-4',
          data: 'Janeiro 04, 2022',
          title: 'Use essas dicas nas suas aplicações mobile',
          text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique.',
        },
      ],
    };
  },
};
</script>

<style scoped>
  @import url("../styles/category.css")
</style>
