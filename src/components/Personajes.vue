<template>
  <div class="background">
      <div v-for="(item, index) in datosPersonajes" :key="index">
        <img :src="item.image" :alt="item.name"><span> {{item.name}}</span>
      </div>
  </div>
</template>

<script>
export default {
 name: 'Personajes',
 props: {
   datosPersonajes: {
     type: Array,
     required: true
   }
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .background {
    padding-top: 20px;
    padding-bottom: 50px;
    background-image: url('../assets/background.png');
    background-size: cover;
  }
  img {
    border-radius: 50%;
    width: 120px;
    margin-bottom: 20px;
    margin-left: 50px;
    margin-right: 50px;
  }
  span {
    color:darkgreen;
    font-family: 'Times New Roman', Times, serif;
    font-size: 30px;
    font-weight: bold;
  }

</style>

