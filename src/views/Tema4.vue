<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5  
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span.txt--white 4
      h1 Desarrollo guiado por pruebas

    .row.justify-content-center.mb-5
      .col-lg-6
        .crd.crd--round.crd--blue(data-aos="flip-left")
            .row.justify-content-end
              .col.mb-4
                figure
                  img(src="@/assets/componentes/quote_r.svg", alt="alt", style="width:41px;")
              .col-12
                p.txt--white El desarrollo de software dirigido por pruebas es una técnica de programación en la cual las pruebas que normalmente son las unitarias se escriben primero y luego se escribe el código que pase la pruebas, con esta práctica se consigue entre otras cosas: un código más robusto, más seguro, más mantenible y una mayor rapidez en el desarrollo.                             
              .col-auto
                .square--orange
      .col-lg-6
        p Cuando el TDD (Desarrollo dirigido por pruebas), se combina con el desarrollo Ágil, según Herranz (2021), tiene como consecuencia un espacio más amplio el cual cubre el desarrollo de #[i software], hasta el diseño de #[i software], el cual propone el proceso denominado:
        .row
          .col-lg-4(data-aos="flip-up")
            .celda.celda--rojo
              h4.mb-0.p-0.txt--white.text-center Rojo
            .celda.celda--gris
              p.mb-0.text-center Hacer que las pruebas fallen
          .col-lg-4(data-aos="flip-up")
            .celda.celda--verde
              h4.mb-0.p-0.txt--white.text-center Verde
            .celda.celda--gris
              p.mb-0.text-center Hacer que las pruebas pasen
          .col-lg-4(data-aos="flip-up")
            .celda.celda--azul
              h4.mb-0.p-0.txt--white.text-center Refactory
            .celda.celda--gris
              p.mb-0.text-center Corregir errores lógicos

    .row.justify-content-center.bg-half--blue_bottom
      .col-lg-10
        .crd.crd--round.crd--yellow
          p.mb-0 Según Sánchez (2017): “Para usar TDD el desarrollador de #[i software] tiene que cambiar su método de trabajo. Ahora, en vez de crear los casos de uso y después implementarlos, va a intentar convertir un caso de uso en un ejemplo. Si se realiza esto con todos los casos de uso, llegará un momento en el que los ejemplos describirán por sí solos la próxima tarea a implementar”.

    .bg--ligthblue
      .row.justify-content-center  
        .col-lg-10.my-5
          p.text-center El proceso de diseño de #[i software], combinando TDD con metodologías ágiles, sería el siguiente:

      .row.justify-content-center.mb-5      
        .col-lg-6.order-2.order-lg-1       
          LineaTiempoD.color-secundario.ltD--color
            p(numero="1" titulo="Historia del usuario") El cliente escribe su historia de usuario.

            p(numero="2" titulo="Aceptación de la historia de usuario") Se definen en conjunto con el cliente los criterios de aceptación de la historia de usuario, descomponiéndola todo lo que se pueda para simplificar lo más posible.

            p(numero="3" titulo="Punto de aceptación") Se selecciona el punto de aceptación más sencillo y se transforma en la prueba unitaria.

            p(numero="4" titulo="Verifica") Se verifica que esta prueba falla.

            p(numero="5" titulo="Prueba correcta") Se escriben las líneas de código para hacer que la prueba sea correcta.

            p(numero="6" titulo="Automático") Se llevan a cabo todas las pruebas de carácter automático. 

            p(numero="7" titulo="Vuelve") Se vuelve a escribir el código para que quede limpio.    

            p(numero="8" titulo="Volvamos al punto 3") Se debe regresar al paso número 3 en cuanto se detecten criterios de aceptación que hagan falta y se debe repetir el ciclo una y otra vez hasta lograr la aplicación completa.   

        .col-lg-5.order-1.order-lg-2.mb-5.mb-lg-0
          figure(data-aos="flip-left")
            img(src="@/assets/curso/tema4/t4_1.svg", alt="alt").m-auto.img350        
       
      .row.justify-content-center
        .col-lg-10
          p Es de comentar que este es un proceso de desarrollo relativamente nuevo, el cual está comenzando a ganar terreno y ser conocido en el ámbito del desarrollo de #[i software] en las organizaciones a nivel mundial, el cual se basa en evidencias anecdóticas y una serie de evaluaciones empíricas. Hablando del desarrollo tradicional las pruebas, se usan para validar y verificar la calidad del #[i software] y su creación se realiza después de que existe la funcionalidad.

          .cajon.cjn--verde.p-4.mb-5        
            p Nota: en el TDD, las pruebas adicionales al tema de validación y verificación se usan con fines de especificar, donde primero se desarrolla la prueba y posteriormente la funcionalidad. Esto permite que la calidad del #[i software] aumente y la productividad del desarrollador mejore, dado que se lleva un mejor esfuerzo en depurar y se avanza rápidamente con el progreso del producto #[i software].

          p.text-center.mb-5 A continuación, se puede observar los beneficios del desarrollo guiado por pruebas:

    .bg-half--blue.mb-5
      .row.justify-content-center
        .col-lg-3(data-aos="flip-up")
          .crd.crd--white.crd--round.crd--shadow.text-center.fullhg
            img(src='@/assets/curso/tema4/t4_3.svg' alt='AvatarTop').mb-4.img90.m-auto
            h4 TDD
            p TDD permite una verificación de las funcionalidades desarrolladas, en ciclos más pequeños, lo que permite la detección de errores y así mismo su solución temprana. 
        .col-lg-3(data-aos="flip-up")
          .crd.crd--white.crd--round.crd--shadow.text-center.fullhg
            img(src='@/assets/curso/tema4/t4_4.svg' alt='AvatarTop').mb-4.img90.m-auto
            h4 Implementación
            p La implementación de esta forma de trabajo permitirá elevar la fiabilidad del producto #[i software], no solo desde el punto de vista de errores funcionales, sino avanzar con las necesidades requeridas por el cliente.
        .col-lg-3(data-aos="flip-up")
          .crd.crd--white.crd--round.crd--shadow.text-center.fullhg
            img(src='@/assets/curso/tema4/t4_5.svg' alt='AvatarTop').mb-4.img90.m-auto
            h4 Optimización
            p Otro de los beneficios es la optimización y mejora en el rendimiento del código, dado que se hace énfasis en escribir solamente el código necesario para la resolución de la necesidad.
        .col-lg-3(data-aos="flip-up")
          .crd.crd--white.crd--round.crd--shadow.text-center.fullhg
            img(src='@/assets/curso/tema4/t4_6.svg' alt='AvatarTop').mb-4.img90.m-auto
            h4 Proceso
            p El proceso de realizar pruebas por cada nueva funcionalidad o requisito facilita el proceso de desarrollo de forma modular, lo que permite la escalabilidad y el futuro mantenimiento del producto #[i software].

    .blackSpace

    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure(data-aos="flip-right")
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Ciclo del desarrollo guiado por pruebas

    p.mb-5 Ahora que ya se saben los beneficios que implica aplicar TDD, es posible ver el ciclo completo del proceso, revisando cada uno de sus pasos. En la siguiente figura se puede observar el flujo de manera gráfica:

    .row.justify-content-center.mb-5
      .col-lg-10
        .titulo-sexto.color-acento-contenido
              h5 Figura 4. 
              span Ciclo TDD
        figure(data-aos="zoom-in")
          img(src="@/assets/curso/tema4/t4_2.svg", alt="alt").m-auto
 
          


    

    

</template>

<script>
export default {
  name: 'Tema4',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
