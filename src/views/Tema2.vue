<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span.txt--white 2
      h1 Tipos de pruebas y sus características

    p En los últimos años se han propuesto algunos principios con el fin de establecer pautas universales para que los programadores de #[i software] las adapten a sus procesos de pruebas.

    .bg-half--blue_bottom
      .row.justify-content-center
        .col-lg-10
          .celda.celda-orange
            h4.text-center.mb-0 Mera (2016), lista los siete principios:
    .bg--gradient
      .row.justify-content-center.pt-5
        .col-lg-10
          PasosA.color-acento-contenido.mb-5(tipo="n")
            .row
              .col-md-8.mb-4.mb-md-0
                h4 Las pruebas muestran la presencia de defectos
                p Las pruebas son herramientas que facilitan detectar defectos; no obstante, no garantizan que no haya defectos ocultos y no es una evidencia de que el #[i software] esté óptimo.
              .col-md-4
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_1.png', alt='Texto que describa la imagen').img160.m-auto

            .row
              .col-md-4.mb-4.mb-md-0
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_2.png', alt='Texto que describa la imagen').img160.m-auto                
              .col-md-8
                h4.t-left Pruebas tempranas
                p.t-left Encontrar los errores en etapas tempranas, permite un importante ahorro de recursos. 

            .row
              .col-md-8.mb-4.mb-md-0
                h4 No es posible realizar pruebas exhaustivas
                p Hay que realizar un análisis de riesgos, para identificar prioridades y tener una óptima toma de decisiones, centralizando esfuerzos y utilizando el talento humano y recursos de manera correcta.
              .col-md-4
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_3.png', alt='Texto que describa la imagen').img160.m-auto
            .row
              .col-md-4.mb-4.mb-md-0
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_4.png', alt='Texto que describa la imagen').img160.m-auto                 
              .col-md-8
                h4.t-left Las pruebas dependen del contexto 
                p.t-left Estas dependen del contexto en el cual se ejecutan; por lo cual se debe dar más énfasis en las que sean para un sistema crítico como para un #[i software] financiero,  para el cual se requiere realizar más pruebas, en comparación con otras aplicaciones con nivel críticos bajos.

            .row
              .col-md-8.mb-4.mb-md-0
                h4 Agrupación de defectos 
                p Las pruebas deben agruparse, la mayoría de fallos operativos se enfocan en un número reducido de módulos.
              .col-md-4
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_5.png', alt='Texto que describa la imagen').img160.m-auto
            .row
              .col-md-4.mb-4.mb-md-0
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_6.png', alt='Texto que describa la imagen').img160.m-auto                 
              .col-md-8
                h4.t-left La paradoja de los pesticidas 
                p.t-left No hay que repetir la misma prueba varias veces,  por lo cual es importante que los casos de prueba se revisen constantemente y escribir nuevos con el fin de encontrar más defectos.

            .row
              .col-md-8.mb-4.mb-md-0
                h4 Ausencia de error
                p De nada sirve corregir en el sistema si este no cumple con los requerimientos o necesidades del usuario.
              .col-md-4
                figure(data-aos="zoom-in")
                  img(src='@/assets/curso/tema2/t2_7.png', alt='Texto que describa la imagen').img160.m-auto

    h3.text-center Ahora, se pueden ver cuáles son los tipos de pruebas que se pueden realizar:    

    .blackSpace

    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Pruebas Funcionales

    p.mb-5 IBM (2021), plantea que estas pruebas se basan en la ejecución y revisión de las funciones y en su interoperabilidad con sistemas específicos, se llevan a cabo en todos los niveles de prueba. Buscan evaluar cada una de las opciones con las que cuenta el paquete informático, principalmente en el comportamiento externo del producto o aplicativo, también se las identifica como de tipo caja negra, ver figura 1.
    
    .row.justify-content-center
      .col-lg-10
        .titulo-sexto.color-acento-contenido
          h5 Figura 1.
          span Pruebas funcionales
        figure(data-aos="flip-right")
          img(src="@/assets/curso/tema2/t2_9.svg", alt="alt").m-auto.img600

    .hr--divider  
    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Pruebas unitarias

    p.mb-5 Las pruebas unitarias o como también se las conocen “#[i Unit testing]”, son pequeños #[i tests] en los cuales se revisa que el comportamiento de un objeto y su lógica funcionen adecuadamente. Por lo general se realiza durante la fase de desarrollo de la aplicaciones o #[i software], esta es ejecutada por los programadores, aunque también pueden realizarlas los aseguradores de calidad.

    .row.justify-content-center.mb-5
      .col-lg-5
        figure(data-aos="flip-left")
          img(src="@/assets/curso/tema2/t2_10.svg", alt="alt").m-auto.img600
      .col-lg-7
        p Las razones por las cuales se desarrollan este tipo de pruebas son:
        ul.lista-ul
          li 
            i.fas.fa-angle-right.clr--blue
            | Son rápidas de realizar por lo que se pueden realizar en gran cantidad. 
          li 
            i.fas.fa-angle-right.clr--blue
            | Demuestran que la lógica del código funciona en todos los casos.   
          li 
            i.fas.fa-angle-right.clr--blue
            | Permite a los programadores entender bien el código base, lo que facilitará realizar cambios oportunos.
          li 
            i.fas.fa-angle-right.clr--blue
            | Se obtendrá un código de calidad.

        p En algunos casos, las pruebas pueden hacerse de manera manual pero lo mejor es usar herramientas que permitan ejecutar el servicio de la mejor manera posible. Existen muchas herramientas en el mercado y estas varían en función del lenguaje de programación que se esté utilizando; aquí se mencionarán algunas de las más conocidas:

    .row.justify-content-center.mb-5
      .col-lg-5
        figure(data-aos="flip-down")
          img(src="@/assets/curso/tema2/t2_11.png", alt="alt").m-auto.img600.mb-4
        h5 xUnit
        p Es una herramienta de pruebas unitarias para el #[i framework.NET].
      .col-lg-5
        figure(data-aos="flip-down")
          img(src="@/assets/curso/tema2/t2_12.png", alt="alt").m-auto.img600.mb-4
        h5 Junit
        p Es una herramienta de pruebas de aplicaciones Java.
      .col-lg-5
        figure(data-aos="flip-down")
          img(src="@/assets/curso/tema2/t2_13.png", alt="alt").m-auto.img600.mb-4
        h5 NUnit
        p Es una herramienta de pruebas de plataformas .NET.
      .col-lg-5
        figure(data-aos="flip-down")
          img(src="@/assets/curso/tema2/t2_14.png", alt="alt").m-auto.img600.mb-4
        h5 PHPUnit
        p Es una herramienta de pruebas de programación PHP.

    .row.justify-content-center.mb-5  
      .col-lg-10
        .banner.banner--azul
          .row.justify-content-center.align-items-center
            .col-auto
              figure(data-aos="flip-left")
                img(src="@/assets/curso/tema2/t2_14.svg", alt="alt").m-auto.img350
            .col
              p Para realizar las pruebas unitarias se deben tener en cuenta los siguientes criterios:
              ul.lista-ul
                li 
                  i.fas.fa-angle-right.clr--blue
                  | Probar un solo código a la vez.
                li 
                  i.fas.fa-angle-right.clr--blue
                  | Hay que realizar pruebas frecuentemente mientras se programa.
                li 
                  i.fas.fa-angle-right.clr--blue
                  | Corregir los bugs identificados en las pruebas antes de continuar.
                li 
                  i.fas.fa-angle-right.clr--blue
                  | Cualquier cambio que se realice también debe pasar la prueba.

    .hr--divider  
    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Pruebas de integración    
      
        
    .row.justify-content-center.align-items-start.mb-5
      .col-lg-7
        p De acuerdo con Mera (2016), estas pruebas son las encargadas de verificar el óptimo acople entre los componentes y de probar las interfaces entre los módulos, como el sistema de archivos en integración con el #[i hardware] y el componente de validación de usuario con el sistema operativo (ver figura 2). Se debe tener en cuenta los objetos típicos de prueba, los cuales son:
        .row.justify-content-center.align-items-center
          .col-lg-6
            figure(data-aos="flip-left")
              img(src="@/assets/curso/tema2/t2_15.svg", alt="alt").m-auto.img450
          .col-lg-6
            ul.lista-ul
              li 
                i.fas.fa-angle-right.clr--blue
                | Bases de datos de subsistemas.
              li 
                i.fas.fa-angle-right.clr--blue
                | Datos de configuración.
              li 
                i.fas.fa-angle-right.clr--blue
                | Configuración del sistema.
              li 
                i.fas.fa-angle-right.clr--blue
                | Infraestructura.
              li 
                i.fas.fa-angle-right.clr--blue
                | Interfaces.
      .col-lg-5
        .titulo-sexto.color-acento-contenido
          h5 Figura 2.
          span Pruebas de integración
        img(src="@/assets/curso/tema2/t2_16.svg", alt="alt").m-auto.img450

    p.mb-5 El mismo autor argumenta que en las pruebas de integración se revisan las interfaces entre componentes o subsistemas, para cerciorarse que son llamados cuando se necesite y que los datos o mensajes que se transmiten son los adecuados. Existen los siguientes tipos de pruebas de integración:

    .row.justify-content-center
      .col-lg-7
        AcordionA.mb-5(tipo="a" clase-tarjeta="tarjeta tarjeta--azul")
          .row(titulo="Integración incremental")            
            p Se prueba el nuevo componente en conjunto con las que ya se probaron y se incrementa progresivamente con los nuevos componentes que se probarán.

          .row(titulo="Descendente")            
            p También conocidas como (#[i top-down]) se realizan siguiendo el flujo de control, ejemplo, desde el GUI o menú principal y los componentes o sistemas se sustituyen por #[i stubs].

          .row(titulo="Ascendente")            
            p También conocidas como (#[i bottom-up]) las pruebas se ejecutan desde la parte inferior del flujo hacia arriba y los componentes o sistemas se sustituyen por controladores.

          .row(titulo="Integración no incremental")            
            p También conocida como #[i Big-bang]  se prueba cada componente por separado y al final se integran todos de una vez realizando las pruebas pertinentes.

          .row(titulo="Combinadas")            
            p Se desarrolla combinando el enfoque ascendente y descendente, pero hay que realizar una planificación para que los componentes individuales se encuentren en el medio. 
    
      
      .col-lg-5(data-aos="flip-right")
        img(src="@/assets/curso/tema2/t2_17.svg", alt="alt").m-auto.img350

    .hr--divider  
    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Pruebas no funcionales

    p.mb-5 En este tipo de pruebas se comprueban los requisitos basados en la operación de un #[i software], no en su funcionalidad. Estas pruebas pueden ayudar a establecer la carga que resiste el producto, si su rendimiento es el adecuado o si es estable a nivel de contacto con el servidor, en otras palabras, no dice si tienen un bajo desempeño o rendimiento en la producción.  Aquí se encuentra:

    .row.justify-content-center.mb-5
      .col-lg-7 
        LineaTiempoD.color-secundario
          p(numero="1" titulo="Pruebas de carga") Simulan la demanda esperada que puede tener una aplicación y mide el resultado.

          p(numero="2" titulo="Pruebas de rendimiento") Se calcula la respuesta del programa con diferentes medidas de peticiones del usuario.

          p(numero="3" titulo="Pruebas de volumen") Se prueba el funcionamiento del programa con ciertos volúmenes de datos.

          p(numero="4" titulo="Pruebas de estrés") Cuantos usuarios o peticiones puede soportar el programa, con esta prueba se determina si el sistema es estable.

      .col-lg-5
        figure(data-aos="flip-right")
          img(src="@/assets/curso/tema2/t2_18.svg", alt="alt").img350.m-auto


    .row.justify-content-center
      .col-lg-5
        figure(data-aos="flip-left")
          img(src="@/assets/curso/tema2/t2_19.svg", alt="alt").img350.m-auto

      .col-lg-7 
        LineaTiempoD.color-secundario
          p(numero="5" titulo="Pruebas de configuración") Aquí se valida qué efectos en el desempeño tienen los cambios de configuración que se pueden aplicar como en diferente #[i hardware], #[i software], versiones y navegadores.

          p(numero="6" titulo="Prueba de resistencia") Aquí se prueba cómo se comporta una aplicación luego de un uso prolongado.

          p(numero="7" titulo="Pruebas de volumen") Se evalúa si la aplicación cumple con los objetivos para el cual fue diseñado.

          p(numero="8" titulo="Pruebas de usabilidad") Se centran en validar que tan fácil se utiliza el programa en cuanto a facilidad de aprendizaje, eficiencia, memorización, errores y satisfacción.    

    .hr--divider  
    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Pruebas de rendimiento

    p Según IBM (2021), estas pruebas  sirven para evaluar lo rápido que el programa realiza una tarea en condiciones específicas de trabajo, también evalúa la escalabilidad, fiabilidad y uso de los recursos.
    p Los objetivos de estas pruebas son:

    .row.justify-content-center
      .col-lg-4  
        .crd--custom(data-aos="flip-right")       
          .imgContainer
            figure
              img(src="@/assets/curso/tema2/t2_20.svg", alt="alt").img160.m-auto
          .bodyContainer
            h4 Identificar y localizar problemas de rendimiento
            p Es permitir encontrar un fallo en el rendimiento, y también ayudar a localizar en qué parte está ese problema de rendimiento para poder solucionarlo.
      .col-lg-4      
        .crd--custom(data-aos="flip-right")   
          .imgContainer
            figure
              img(src="@/assets/curso/tema2/t2_21.svg", alt="alt").img160.m-auto
          .bodyContainer
            h4 Verificar el cumplimiento de los SLA (Acuerdos de Nivel de Servicio)
            p Se utiliza para medir los tiempos de respuesta del #[i software] en condiciones y tiempos específicos.
      .col-lg-4   
        .crd--custom(data-aos="flip-right")     
          .imgContainer
            figure
              img(src="@/assets/curso/tema2/t2_22.svg", alt="alt").img160.m-auto
          .bodyContainer
            h4 Localizar cuellos de botella
            p Ayudar a detallar en qué lugar se generan estos cuellos de botellas si se debe problemas de #[i hardware] como CPU, memoria, o es el ancho de banda.

    .hr--divider  
    .cstm--title.mb-4    
      .row.align-items-center
        .col-auto
          figure
            img(src="@/assets/componentes/title_icon.svg", alt="alt").img90.m-auto
        .col 
          h3.mb-0 Ventajas y desventajas de los tipos de pruebas 

    p.mb-5 Todo proceso tiene sus ventajas y desventajas, a continuación se presentan cada una de ellas.

    h3.mb-5 Ventajas de estos tipos de pruebas

    .row.justify-content-center
      .col-lg-7
        
        AcordionA.mb-5(tipo="a" clase-tarjeta="tarjeta tarjeta--gris")
          .row(titulo="Pruebas funcionales")                
            ul.list--cs.mb-2
              li
                i.fas.fa-angle-right.clr--blue
                | Optimiza las funcionalidades y la calidad del producto.
              li 
                i.fas.fa-angle-right.clr--blue
                | Verifica que la seguridad y la arquitectura sean las adecuadas.
              li 
                i.fas.fa-angle-right.clr--blue
                | Asegura que el comportamiento del <em>software</em> y de todas sus funciones sea el esperado.
              li 
                i.fas.fa-angle-right.clr--blue
                | Se asegura que el <em>software</em> o aplicación está libre de errores.

          .row(titulo="Pruebas unitarias")    
            ul.list--cs.mb-2
              li
                i.fas.fa-angle-right.clr--blue
                | Simplifica la integración y permite una buena documentación.
              li
                i.fas.fa-angle-right.clr--blue
                | Funciona con el  proceso de desarrollo ágil.
              li
                i.fas.fa-angle-right.clr--blue
                | Detección temprana de errores en sus funcionalidades lo que minimiza tiempo y costos.
              li
                i.fas.fa-angle-right.clr--blue
                | Optimiza la efectividad del código.
           

          .row(titulo=" Pruebas de integración")     
            ul.list--cs.mb-2
              li
                i.fas.fa-angle-right.clr--blue
                | Detalla los errores y conflictos en cada módulo y en sus conexiones.
              li
                i.fas.fa-angle-right.clr--blue
                | Mejora la calidad del código.
              li
                i.fas.fa-angle-right.clr--blue
                | Garantiza que las funciones del <em>software</em> serán confiables y estables entres sus módulos.
              li
                i.fas.fa-angle-right.clr--blue
                | Garantiza que todos los módulos del <em>software</em> estén correctamente integrados y funcionen en conjunto como se necesita.
            

          .row(titulo="Pruebas de Rendimiento")       
            ul.list--cs.mb-2
              li
                i.fas.fa-angle-right.clr--blue
                | Mejora las características del <em>software</em> o aplicación perfeccionando el sistema.
              li
                i.fas.fa-angle-right.clr--blue
                | Identifica errores que no se detectan en las pruebas funcionales.
              li
                i.fas.fa-angle-right.clr--blue
                | Localiza los cuellos de botella para solucionarlos y optimizar su rendimiento.
              li
                i.fas.fa-angle-right.clr--blue
                | Valora la escalabilidad y velocidad de la aplicación o <em>website.</em>    
                     
            

      .col-lg-5
        figure(data-aos="flip-right")
          img(src="@/assets/curso/tema2/t2_23.svg", alt="alt").m-auto.img350

    h3.mb-5 Desventajas de estos tipos de pruebas:
    p Por lo general, todas las pruebas de #[i software] traen beneficios al desarrollador, dependiendo del tipo de la prueba los beneficios pueden ser más altos y enfocados en un fin o propósito especifico, dando como resultado una mejor calidad de producto, mejorando su funcionalidad, reduciendo costos, tiempos, recursos humanos y mejorando la experiencia del usuario.
    p.mb-5 Se podría considerar como una desventaja, si se comparan los tipos de prueba ya que puede variar en:


    .bg--ligthblue
      .row.justify-content-center.pt-5
        .col-auto.mb-4
          img(src='@/assets/curso/tema2/t2_24.svg' alt='AvatarTop').img250.m-auto(data-aos="flip-right")
        .col-auto.mb-4
          img(src='@/assets/curso/tema2/t2_25.svg' alt='AvatarTop').img250.m-auto(data-aos="flip-right")
        .col-auto.mb-4
          img(src='@/assets/curso/tema2/t2_26.svg' alt='AvatarTop').img250.m-auto(data-aos="flip-right")
      .row.justify-content-center    
        .col-auto.mb-4
          img(src='@/assets/curso/tema2/t2_27.svg' alt='AvatarTop').img250.m-auto(data-aos="flip-right")
        .col-auto.mb-4         
          img(src='@/assets/curso/tema2/t2_28.svg' alt='AvatarTop').img250.m-auto(data-aos="flip-right")
    .bg-half--blue
      .row.justify-content-center
        .col-lg-10
          .crd.crd--yellow.crd--round
            p.mb-0 Sin embargo, la única desventaja de las pruebas de #[i software] son no hacerlas ya que el omitir este paso desencadena una nefasta serie de errores como un producto no funcional y colocarían en tela de juicio la profesionalidad de programador y su equipo de trabajo.
            



      


      







  

            




            
                
                  


    
    

</template>

<script>
export default {
  name: 'Tema2',
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
