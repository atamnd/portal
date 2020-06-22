<template>
  <v-app>
    <Header />
    <v-content id="main" class="main">
      <router-view></router-view>
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'

export default {
  name: 'App',

  components: {
    Header,
    Footer
  },

  data() {
    return {

    };
  },
  mounted() {
    const header = document.getElementById('header');
    const height = header.clientHeight;
    const target = document.getElementById('main');
    target.style.paddingTop = (height * 2) + 'px';
    target.style.paddingBottom = height + 'px';
  },
};
</script>