<template>
  <div id="aboutus">
    <section class="section-info-1">
      <div class="section-info-col-1">
        <div class="content-info-1">
          <img :src="images.post1" :alt="images.alt" />
          <p>{{content.dataSectionOne}}</p>
        </div>
        <div class="content-info-2">
          <h3>{{content.titleSectionOne}}</h3>
          <p>{{content.textSectionOne}}</p>
        </div>
      </div>
    </section>

    <section class="section-info-2">
      <div class="content-info-1">
        <p>{{content.dataOneSectionTwo}}</p>
        <h3>{{content.titleOneSectionTwo}}</h3>
        <p>{{content.textOneSectionTwo}}</p>
      </div>

      <div class="content-info-1">
        <p>{{content.dataTwoSectionTwo}}</p>
        <h3>{{content.titleTwoSectionTwo}}</h3>
        <p>{{content.textTwoSection2}}</p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images:
      {
        // eslint-disable-next-line global-require
        post1: require('../assets/images/post-1.png'),
        alt: 'Imagem do post-1',
      },
      content:
      {
        dataSectionOne: 'Janeiro 04, 2022',
        titleSectionOne: 'Começando no ReactJS em 2022',
        textSectionOne: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique. Sed volutpat aenean.',
        dataOneSectionTwo: 'Janeiro 04, 2022',
        titleOneSectionTwo: 'Conheça as principais técnicas para conseguir uma vaga internacional em programação',
        textOneSectionTwo: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. Sed volutpat aenean sit vitae, sed tristique.',
        dataTwoSectionTwo: 'Janeiro 04, 2022',
        titleTwoSectionTwo: 'Veja a evolução do Front-end na prática',
        textTwoSection2: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nibh nibh eu in aliquet ut adipiscing neque. ',

      },
    };
  },
};
</script>

<style>
  @import url("../styles/aboutUs.css")
</style>
