<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5 

    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 
          i.fas.fa-info.txt--white
      h1 Introducción

    p.mb-4 Las pruebas del software son un grupo de actividades enfocadas en encontrar los posibles fallos en el funcionamiento de todo software. Se invita a ver el siguiente video para conocer de qué tratará el componente formativo.
    
    figure.mb-5
      .video
        iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)  
   

</template>

<script>
export default {
  name: 'Introduccion',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
