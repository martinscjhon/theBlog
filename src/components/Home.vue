<template>
  <div id="home">
    <section class="content">
      <div class="text">
        <div>
          <h1>{{title}}</h1>
          <p>{{subTitle}}</p>

            <div class="saiba-mais">
              <a href="">
                <h3>{{linkVejaMais}}</h3>
                <img :src="images[0].arrow" :alt="images[0].alt" />
              </a>
            </div>
        </div>
      </div>

        <div class="image-content">
          <img :src="images[1].post" :alt="images[1].alt">
        </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'HomeComponent',
  data() {
    return {
      title: 'Veja o guia definitivo para conquistar seus objetivos como DEV em 2022',
      subTitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique placerat hac.',
      linkVejaMais: 'Veja mais',
      images: [
        {
          // eslint-disable-next-line global-require
          arrow: require('../assets/images/arrow-right.svg'),
          alt: 'imagem da seta saiba mais',
        },
        {
          // eslint-disable-next-line global-require
          post: require('../assets/images/featured-image.png'),
          alt: 'imagem do post-1',
        },
      ],
    };
  },
};
</script>

<style scoped>
  @import url("../styles/home.css")
</style>
