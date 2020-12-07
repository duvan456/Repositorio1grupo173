<template>
  <div id="app">
    <the-carousel></the-carousel>
    <div class="container-fluid">
      <div class="row justify-content-center mb-5">        
        <div class="col mt-5" v-for="(item,index) of team" :key="index">
          <div id="equipo">
            <team-card :member="item"></team-card>
          </div>
        </div>         
      </div>
    </div>
  </div>
</template>

<script>

import TeamCard from './components/TeamCard.vue'
import TheCarousel from "./components/TheCarousel.vue"

export default {
  name: 'App',
  components: {
    TeamCard,
    TheCarousel
  },
  data(){
    return{
      team: [
       {
        codigo : 1 ,
        nombre : 'Oscar Jimenez' ,
        descripcion : "Ingeniero de Petróleos, 26 años, sus pasatiempos son la fotografia y los videojuegos",
        rol : "Desarrollador backend",
        imagen : require('./assets/Oscar_opt.jpg')
        },
               {
        codigo : 2 ,
        nombre : 'Duvan Ceron' ,
        descripcion : "Estudiante de contaduria pública, 22 años, su pasatiempos es viajar",
        rol : "Desarrollador backend",
        imagen : require('./assets/Duvane_opt.jpg')
               },
        {
        codigo : 3 ,
        nombre : 'Felipe Pinto' ,
        descripcion : "Estudiante de ingenieria sanitaria, 20 años, su pasatiempos es jugar microfutbol",
        rol : "Desarrollador backend",
        imagen : require('./assets/Felipe_opt.jpg')
        },
        {
        codigo : 4,
        nombre : 'Cindy Figuera' ,
        descripcion : "Ingenieria de Sistemas, 39 años, su pasatiempos es jugar golosa",
        rol : "Desarrollador backend",
        imagen : require('./assets/Cindy.jpg')
        },
        {
        codigo : 5 ,
        nombre : 'Wilder Erazo' ,
        descripcion : "Estudiante de ingenieria industrial, 25 años, su pasatiempos es jugar baloncesto",
        rol : "Desarrollador backend",
        imagen : require('./assets/Wilder_opt.jpg')
        },
      ]
    }
  }
}
</script>