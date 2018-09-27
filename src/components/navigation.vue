<template>
  <nav class="menu-navigation">
      <a :href="link.link" v-for="link in links" :key="link.text">
        {{ link.text }}
      </a>


      <span @click="open">&#9776;</span>
  </nav>
</template>

<script>
export default {
  name: 'menuNavigation',
  data() {
    return {
      links: [
        {
          text: 'Главная',
          link: '#'
        },
        {
          text: 'Витрина',
          link: '#'
        },
        {
          text: 'Контакты',
          link: '#'
        },
        {
          text: 'О нас',
          link: '#'
        },
        {
          text: 'Купить оптом',
          link: '#'
        }
      ]
    };
  },
  methods: {
    open() {
      console.log('Open menu');
    }
  }
}
</script>

<style scoped>

.menu-navigation a {
  color: #42b983;
  text-decoration: none;
}

</style>
