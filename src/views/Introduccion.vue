<template lang="pug">
.curso-main-container.introduccion
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span
          i.fas.fa-info
      h1 Introducción
    

    .row.justify-content-center.mb-5
      .col-sm-12.col-lg-7
          p.mb-3 El patronaje de prendas deportivas infantiles exige una articulación precisa entre el conocimiento de las proporciones del cuerpo en crecimiento, las propiedades técnicas de los materiales textiles y los criterios funcionales propios de la actividad física. Para el rango etario de 6 a 12 años, estas variables adquieren una dimensión particular: el cuerpo se encuentra en transformación morfológica activa, los tejidos de punto predominan en la construcción de las prendas y las exigencias de movimiento, ajuste y durabilidad condicionan cada decisión técnica del patronista desde el primer trazo.
          .row.justify-content-center.mb-0
            .col-sm-12.col-lg-2.d-none.d-lg-block
              img(src='@/assets/curso/temas/intro/2.svg', alt='')
            .col-sm-12.col-lg-10
                p.mb-0 A partir de este contexto, el presente componente formativo integra el estudio de tipologías representativas del vestuario deportivo infantil (camiseta, camisilla, camiseta manga ranglán, sudadera de punto y mallas) con los fundamentos metodológicos del escalado industrial de patrones.   
      .col-sm-12.col-lg-5.d-none.d-lg-block
        img(src='@/assets/curso/temas/intro/1.png', alt='')

    p.mb-5 La construcción de cada tipología se aborda con planos de trazado, fórmulas de proporción y convenciones técnicas orientadas a la producción, mientras que el escalado se desarrolla desde sus bases conceptuales hasta la aplicación de los métodos bibásico, monobásico y por coordenadas, con énfasis en la separación de tallas y la marcación de patrones para su uso en entornos industriales. El dominio de los contenidos aquí desarrollados sienta las bases técnicas para abordar con rigor los procesos de patronaje industrial del vestuario deportivo infantil. 
    .row.justify-content-center.align-items-center           
      .col-lg-12
        figure
          .video
            iframe(width="560" height="315" src="https://www.youtube.com/embed/vdPrCjWJSHo?si=X4NxENRo3LLXAua_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
        figcaption Video. 

</template>

<script>
export default {
  name: 'Introduccion',
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
