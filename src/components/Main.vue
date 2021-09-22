<template>

  <div class="container">

    <div :key="record.datasetid" v-for="record in data.records">
      <p>Commune : {{ record.fields.commune }}</p>
      <p>Disponible : {{ record.fields.dispo }}</p>
      <div class="flex">
        <p v-if="record.fields.no_voirie_pair">{{ record.fields.no_voirie_pair }} </p>
        <p v-if="record.fields.no_voirie_impair">{{ record.fields.no_voirie_impair }} </p>
        <p>{{ record.fields.voie }}</p>
      </div>
      <p>Coordonnées : {{ record.geometry.coordinates[0] }} - {{ record.geometry.coordinates[1] }}</p>

    </div>


  </div>

</template>

<script>
export default {
  name: "main.vue",

  data() {
    return {
      data: {}
    }
  },
  beforeMount(){
    this.getApiResponse();
  },
  methods: {
    async getApiResponse(){
      const res = await fetch('https://opendata.paris.fr/api/records/1.0/search/?dataset=fontaines-a-boire&q=&facet=type_objet&facet=modele&facet=commune&facet=dispo');
      const data = await res.json();
      this.data = data;
    }
  }
}


</script>

<style scoped>
  .container{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    font-family: Avenir, Helvetica, Arial, sans-serif;

  }
  .container>div{
    width: 30%;
    margin-bottom: 3%;
    border-radius: 5px;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;

  }
  .flex{
    display: flex;
    justify-content: center;
  }
</style>