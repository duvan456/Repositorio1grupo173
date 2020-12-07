<template>
  <div id="app">
    <the-carousel></the-carousel>
    <div id="noticias">
      <div class="container-fluid">
        <the-api></the-api>
      </div>
    </div>
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

import TeamCard from './components/TeamCard.vue';
import TheCarousel from "./components/TheCarousel.vue";
import TheApi from "./components/TheApi.vue";

export default {
  name: 'App',
  components: {
    TeamCard,
    TheCarousel,
    TheApi
  },
  data(){
    return{
      team: [
       {
        codigo : 1 ,
        nombre : 'Oscar Jimenez' ,
        descripcion : "Ingeniero de petróleos, 26 años, sus pasatiempos son la fotografía y los videojuegos",
        rol : "Desarrollador Back end",
        imagen : require('./assets/Oscar_opt.jpg')
        },
               {
        codigo : 2 ,
        nombre : 'Duvan Ceron' ,
        descripcion : "Contador público, 22 años, su pasatiempo es viajar",
        rol : "Desarrollador Front end",
        imagen : require('./assets/Duvane_opt.jpg')
               },
        {
        codigo : 3 ,
        nombre : 'Felipe Pinto' ,
        descripcion : "Estudiante de ingeniería sanitaria, 20 años, su pasatiempo es jugar microfútbol",
        rol : "Desarrollador Front end",
        imagen : require('./assets/Felipe_opt.jpg')
        },
        {
        codigo : 4,
        nombre : 'Cindy Figuera' ,
        descripcion : "Ingeniera de sistemas, 39 años, su pasatiempo es jugar golosa",
        rol : "Desarrolladora Back end",
        imagen : require('./assets/Cindy.jpg')
        },
        {
        codigo : 5 ,
        nombre : 'Wilder Erazo' ,
        descripcion : "Estudiante de ingeniería industrial, 25 años, su pasatiempo es jugar baloncesto",
        rol : "Desarrollador Back end",
        imagen : require('./assets/Wilder_opt.jpg')
        },
      ]
    }
  }
}
</script>