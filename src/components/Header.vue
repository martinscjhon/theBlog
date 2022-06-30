<template>
  <div class="header">
    <header>
      <div>
        <img src="" alt="" />
      </div>

      <nav>
        <ul>
          <li><a href="">Home</a></li>
          <li><a href="">Sobre</a></li>
          <li><a href="">Categorias</a></li>
          <li><a href="">Contato</a></li>
        </ul>
      </nav>

      <div>
        <input />
        <button>
          <img src="" alt="" />
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
      images:
        {
          logo: 'src/assets/images/logo.svg',
          alt: 'Logo da imagem',
        },

    };
  },
};
</script>

<style scoped>

</style>
