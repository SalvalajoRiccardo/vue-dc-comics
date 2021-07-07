<template>
  <div id="app">
    <Header/>
    <main>
      <MainContent/>
      <BlueCutter/>
    </main>
    <Footer/>
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import BlueCutter from './components/BlueCutter.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    BlueCutter,
    Footer
  }
}
</script>

<style lang="scss">
  @import 'styles/Commons.scss';
</style>
