<template>
  <Navbar />
  <Landing />
  <Footer />
</template>

<script>
import Landing from './components/Landing.vue';
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Landing,
    Footer,
  },
};
</script>

<style></style>
