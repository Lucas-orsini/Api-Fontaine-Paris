<template>
  <NavBar></NavBar>
  <div id="app">
    {{data}}
  </div>
  <Footer></Footer>
</template>

<script>
import NavBar from './components/NavBar'
import Footer from './components/Footer'

export default {
  name: "App",
  components:{
    NavBar,
    Footer
  },
  data() {
    return {
      data: {}
    }
  },
  beforeMount(){
    this.getName();
  },
  methods: {
    async getName(){
      const res = await fetch('https://opendata.paris.fr/api/records/1.0/search/?dataset=fontaines-a-boire&q=&facet=type_objet&facet=modele&facet=commune&facet=dispo');
      const data = await res.json();
      this.data = data;
    }
  }
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
