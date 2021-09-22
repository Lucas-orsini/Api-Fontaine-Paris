<template>
  <NavBar></NavBar>
  <div id="app">
    <Main></Main>
  </div>
  <Footer></Footer>
</template>

<script>



import NavBar from './components/NavBar'
import Footer from './components/Footer'
import Main from './components/Main'

export default {
  name: "App",
  components:{
    NavBar,
    Footer
    Main,
  },

};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
