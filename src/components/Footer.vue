<template>
  <div id="footer">
    <div class="container">
      <div>
        <button>
          <img :src="image.logo" :alt="image.alt" />
        </button>
      </div>

      <div class="social-midia">
        <div v-for="footerInfo in footerInfo" :key="footerInfo.icon">
          <div>
            <img :src="footerInfo.icon" :alt="footerInfo.alt" />
          </div>
          <h4>{{footerInfo.description}}</h4>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterComponent',
  data() {
    return {
      image: {
        // eslint-disable-next-line global-require
        logo: require('../assets/images/logo.svg'),
        alt: 'logo-the-blog',
      },
      footerInfo: [
        {
          // eslint-disable-next-line global-require
          icon: require('../assets/images/whatsapp.png'),
          alt: 'icon-whatsapp',
          description: 'WhatsApp',
        },
        {
          // eslint-disable-next-line global-require
          icon: require('../assets/images/instagram.png'),
          alt: 'icon-intagram',
          description: 'Intagram',
        },
        {
          // eslint-disable-next-line global-require
          icon: require('../assets/images/youtube.png'),
          alt: 'icon-youtube',
          description: 'Youtube',
        },
        {
          // eslint-disable-next-line global-require
          icon: require('../assets/images/linkedin.png'),
          alt: 'icon-linkedin',
          description: 'Linkedin',
        },
      ],
    };
  },
};
</script>

<style scoped>
  @import url("../styles/footer.css")
</style>
