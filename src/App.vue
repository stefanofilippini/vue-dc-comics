<template>
  <div id="app">
    <Header/>
    <Content/>
    <Merch/>
    <Contacts/>
    <Footer/>
<!-- 
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
-->
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'
import Merch from '@/components/Merch.vue'
import Footer from '@/components/Footer.vue'
import Contacts from '@/components/Contacts.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Merch,
    Footer,
    Contacts
  }
}
</script>

<style lang="scss">
@import '@/styles/global.scss';

</style>