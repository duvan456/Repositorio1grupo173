<template>
    <div>
        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
            <ol class="carousel-indicators">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
            </ol>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="../assets/carousel-image-1.jpg" class="d-block w-100" height="700">
                    <div class="carousel-caption d-none d-md-block">
                        <h3>Vuelos</h3>
                        <p>Descubre a Colombia y al Mundo Realizando Viajes Con los Vuelos Que Ofrecemos. Encuentra Aerolíneas Tradicionales Y De Bajo Costo En Nuestra Web. Comprueba Buenas Ofertas En Vuelos A Numerosos Aeropuertos Aquí.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="../assets/carousel-image-2.jpg" class="d-block w-100" height="700">
                    <div class="carousel-caption d-none d-md-block">
                        <h3>Alojamiento</h3>
                        <p>Elige alojamientos con reserva flexible, vas a poder cancelar gratis si cambias de planes. Contamos con una amplia oferta de alojamientos de acuerdo a tu presupuesto en todas las ciudades de Colombia y el Mundo.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src='../assets/carousel-image-3.jpg' class="d-block w-100" height="700">
                    <div class="carousel-caption d-none d-md-block">
                        <h3>Tour</h3>
                        <p>Un tour es un itinerario que contempla visitas a diferentes lugares muy caracteristicos de la ciudad de tu preferencia. Te ofrecemos el tour soñado para que tu visita sea inolvidable!</p>
                    </div>
                </div>
            </div>
            <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </div>
</template>

<script>

export default {
    name: "TheCarousel"
    }

</script>

<style scoped>

</style>