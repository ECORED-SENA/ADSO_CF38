<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span.txt--white 1
      h1 Generalidades de las pruebas de software

    p Las pruebas software son parte fundamental del proceso de calidad y adopción de buenas prácticas, estas deben realizarse en todo el proceso de desarrollo de software, de acuerdo con Mera (2016) este proceso debe incluir:

    .bg--ligthblue
      .row.position-relative.py-5
        .col-lg-6
          .crd.crd--round.crd--blue(data-aos="flip-left")
            .row.justify-content-end
              .col.mb-4
                figure
                  img(src="@/assets/componentes/quote_r.svg", alt="alt", style="width:41px;")
              .col-12
                p.txt--white Revisión de los requerimientos, realización de análisis documentales, identificación de defectos, pruebas funcionales y no funcionales, pruebas dinámicas y estáticas, pruebas de integración, informes de confianza en el nivel de calidad, información para la toma de decisiones, planes de mejora continua.
              .col-auto
                .square--orange
        .col-lg-6
          figure(data-aos="zoom-in")
            img(src="@/assets/curso/tema1/t1.svg", alt="alt").m-auto.img350

      p El mismo autor afirma que dentro de las actividades de un proceso de prueba se debe incluir las siguientes fases:

      .row.justify-content-center.my-5
        .col-8.col-lg-4.mb-4
          .crd_container(data-aos="flip-up")
            .crd_container__icon
              figure
                img(src="@/assets/curso/tema1/t2.svg", alt="alt", style="width:110px;").m-auto
            .crd_container__body
              h5 El control
        .col-8.col-lg-4.mb-4
          .crd_container(data-aos="flip-up")
            .crd_container__icon
              figure
                img(src="@/assets/curso/tema1/t2.svg", alt="alt", style="width:110px;").m-auto
            .crd_container__body
              h5 Comprobación de resultados
        .col-8.col-lg-4.mb-4
          .crd_container(data-aos="flip-up")
            .crd_container__icon
              figure
                img(src="@/assets/curso/tema1/t2.svg", alt="alt", style="width:110px;").m-auto
            .crd_container__body
              h5 Elaboración de informes de proceso
        .col-8.col-lg-4.mb-4
          .crd_container(data-aos="flip-up")
            .crd_container__icon
              figure
                img(src="@/assets/curso/tema1/t2.svg", alt="alt", style="width:110px;").m-auto
            .crd_container__body
              h5 Aplicación objeto de las pruebas
        .col-8.col-lg-4.mb-4
          .crd_container(data-aos="flip-up")
            .crd_container__icon
              figure
                img(src="@/assets/curso/tema1/t2.svg", alt="alt", style="width:110px;").m-auto
            .crd_container__body
              h5 Bitácoras de experiencias

    .row.justify-content-center.bg-half--blue.mb-5
      .col-lg-10
        .crd.crd--round.crd--yellow
          p.mb-0 Es de suma importancia realizar una bitácora y una matriz con el fin de ejecutar los casos de prueba y así concluir si el caso funciona como se esperaba:

    .row.justify-content-center
      .col-10
        .row.justify-content-center.mb-5
          .col-auto.mb-4
            figure(data-aos="zoom-in")
              img(src="@/assets/curso/tema1/t3.svg", alt="alt").m-auto.img350
          .col-auto.mb-5
            figure(data-aos="zoom-in")
              img(src="@/assets/curso/tema1/t4.svg", alt="alt").m-auto.img350
          .col-10.mb-5        
            p La matriz ayudan a establecer métricas que ayudan a definir tiempos, esfuerzos, asignaciones, y riesgos logrando optimizar recursos y talento humano.
          .col-auto
            figure(data-aos="zoom-in")
              img(src="@/assets/curso/tema1/t5.svg", alt="alt").m-auto
      .col-10
        .crd.crd--round.crd--shadow 
          .row.justify-content-center
            .col-auto.mb-lg-5.mb-xl-0
              figure(data-aos="zoom-in")
                img(src="@/assets/curso/tema1/t6.svg", alt="alt").m-auto.img350
            .col-md-12.col-xl-8
              h4 Según la organización ISO (2020):
              p Estas pruebas se regulan por la norma ISO/IEC 25000 Sistemas y Requisitos de Calidad y Evaluación de Software (SQuaRE). 
              p Pruebas de software aplicables a todos aquellos que deseen crear: 
              ul.lista-ul
                li 
                  i.fas.fa-angle-right.clr--blue
                  | Especificaciones de prueba. 
                li 
                  i.fas.fa-angle-right.clr--blue
                  | Marcos correspondientes.  
                li 
                  i.fas.fa-angle-right.clr--blue
                  | O crear automatización de pruebas.
            












            


    
  
</template>

<script>
export default {
  name: 'Tema1',
  components: {},
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
