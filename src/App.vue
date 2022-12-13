<template>
  <Header></Header>
  <Main></Main>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
export default {
  name: 'App',
  components: {
    Header,
    Main
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  display:flex;
  flex-direction: column;
  height:100%;
}
html,body { height:100%; }
</style>
