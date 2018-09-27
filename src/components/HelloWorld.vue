<template>
  <!-- Первый блок (Шапка)-->
  <header>
    <div class="header__logo">
      <p>Мясная лавка</p>
    </div>
    <menu-navigation></menu-navigation>

  </header>
</template>

<script>
import menuNavigation from './navigation';

export default {
  name: 'HelloWorld',
  components: {
    menuNavigation
  },
  data() {
    return {

    };
  },
  mounted() {
    console.log('Компонет создался');
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

</style>
