<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5 
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span.txt--white 3
      h1 Los casos de pruebas

    p.mb-5 Son los documentos de los productos que se generan al momento de realizar una prueba de software, en el cual se plasma las precondiciones entradas y resultados esperados, incluyendo la implementación correcta, la identificación de errores, el chequeo de la calidad y otras informaciones consideradas importantes, en general no hay una plantilla especifica solo la bitácora, listas de chequeo, e imágenes en la cual se registran las no conformidades que se encuentran en las pruebas (ver figura 3).

    .row.justify-content-center.mb-5  
      .col-auto
        .titulo-sexto.color-acento-contenido
          h5 Figura 3.
          span Pruebas de integración
        figure(data-aos="zoom-in")
          img(src="@/assets/curso/tema3/t3_1.svg", alt="alt").m-auto.img900

    .bg--ligthblue.mb-5
      .row.justify-content-center.align-items-center.py-5
        .col-auto
          figure(data-aos="flip-right")
            img(src="@/assets/curso/tema3/t3_2.svg", alt="alt").m-auto.img350

        .col
          p En el diseño de las pruebas de software se deben identificar y describir casos de prueba, por lo tanto para documentar un caso de pruebas se debe comprender que este contiene un conjunto de variables o condiciones en la cual un tester determina si un sistema funciona según lo esperado; así mismo, cabe resaltar que la documentación de un caso de prueba se convierte en una actividad sin dificultad, si se tiene la información necesaria para su proceso de elaboración, teniendo en cuenta que al momento de probar un software es de mucho aporte, puesto que se transforma en una herramienta esencial en el proceso de registro, seguimiento y control.
          p A continuación, se nombran los elementos principales que debe contener un caso de prueba (ver tabla 1): 

    tabla-b.my-5
      .tabla-b__header.table--azul
        h5.mb-0 Caso de pruebas
      table        
        tr
          th(width="25%") Identificador
          td Puede ser alfanumérico o numérico.
        tr
          th Nombre
          td Nombre del caso de prueba de manera concisa.
        tr
          th Descripción
          td Objetivo del caso de prueba, también describe que probara, en ciertas ocasiones se incluye el ambiente de pruebas.
        tr
          th Número de orden Ejecución
          td Orden en la cual se ejecuta el caso de prueba, en la situación de que se tengan múltiples casos de prueba.
        tr
          th Requerimiento asociado
          td Si se plantea un caso de prueba se debe saber a qué requerimiento va asociado para mantener la trazabilidad.
        tr
          th Precondición
          td Estado en la cual se debe encontrar el sistema antes de comenzar la prueba.
        tr
          th Postcondición
          td El estado en que debe encontrarse el sistema luego de ejecutar la prueba.
        tr
          th Resultado esperado
          td Objetivo que debe ser alcanzado posterior a ejecutarse la prueba.



    

</template>

<script>
export default {
  name: 'Tema3',
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
