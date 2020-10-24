<template>
  <div>
   <Personajes />
   <personajes :datosPersonajes = "datosPersonajes"></personajes>
  </div>
</template>

<script>
import Personajes from './components/Personajes.vue'
export default {
  name: 'App',
  components: {
    Personajes
  },
  data() {
   return {
     datosPersonajes: [
       {name: "Rick Sanchez", image: "https://rickandmortyapi.com/api/character/avatar/1.jpeg"},
       {name: "Morty Smith", image: "https://rickandmortyapi.com/api/character/avatar/2.jpeg"},
       {name: "Summer Smith", image: "https://rickandmortyapi.com/api/character/avatar/3.jpeg"},
       {name: "Beth Smith", image: "https://rickandmortyapi.com/api/character/avatar/4.jpeg"},
       {name: "Jerry Smith", image: "https://rickandmortyapi.com/api/character/avatar/5.jpeg"}
     ]
   }
 },
}
</script>

<style>

</style>
