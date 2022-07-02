<template>
  <div id="header">
    <header>
      <div>
        <img :src="images[0].logo" :alt="images[0].alt" />
      </div>

      <nav>
        <ul>
          <li><a href="">{{links.name.home}}</a></li>
          <li><a href="">{{links.name.aboutUs}}</a></li>
          <li><a href="">{{links.name.category}}</a></li>
          <li><a href="">{{links.name.contact}}</a></li>
        </ul>
      </nav>

      <div class="search">
        <label
          for="input-search"
          class="sr-only"
          >
            Buscar
          </label>
        <input
          type="text"
          placeholder="Buscar"
          id="input-search"
        />
        <button>
          <img :src="images[1].icon" :alt="images[1].alt" />
        </button>
      </div>
    </header>
  </div>
</template>

<script>

export default {
  name: 'HeaderComponent',
  data() {
    return {
      images: [
        {
          // eslint-disable-next-line global-require
          logo: require('../assets/images/logo.svg'),
          alt: 'logo-the-blog-header',
        },
        {
          // eslint-disable-next-line global-require
          icon: require('../assets/images/search.svg'),
          alt: 'icon-serach-header',
        },
      ],
      links: {
        name: {
          home: 'Home',
          aboutUs: 'Sobre',
          category: 'Categorias',
          contact: 'Contato',
        },
      },
    };
  },
};
</script>

<style scoped>
  @import url("../styles/header.css")
</style>
