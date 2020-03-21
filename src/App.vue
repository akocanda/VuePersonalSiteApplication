<template>
  <div id="app">
    <Header />
    <AboutMe />
    <Skills />
    <Footer />
  </div>
</template>

<script>
import AboutMe from './components/aboutMe/AboutMe.vue'
import Footer from './components/footer/Footer.vue'
import Skills from './components/skills/Skills.vue'
import Header from './components/header/Header.vue'

export default {
  name: 'App',
  components: {
    AboutMe,
    Footer,
    Skills,
    Header
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
