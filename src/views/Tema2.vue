<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
      .titulo-principal.color-acento-contenido
        .titulo-principal__numero
          span 2
        h1 Escalado de prendas de vestir
      #t_2_1.titulo-segundo.color-acento-contenido(data-aos='fade-right')
        h2 2.1 Concepto y objetivos del escalado
      #t_2_2.titulo-segundo.color-acento-contenido(data-aos='fade-right')
        h2 2.2 Principios técnicos del escalado en prendas de vestir
      #t_2_3.titulo-segundo.color-acento-contenido(data-aos='fade-right')
        h2 2.3 Tipos de escalado: proporcional, combinado y diferencial
      #t_2_4.titulo-segundo.color-acento-contenido(data-aos='fade-right')
        h2 2.4 Escalado bibásico
      #t_2_5.titulo-segundo.color-acento-contenido(data-aos='fade-right')
        h2 2.5 Escalado monobásico y por coordenadas
      #t_2_6.titulo-segundo.color-acento-contenido(data-aos='fade-right')
        h2 2.6 Separación de tallas y marcación
      
        

  </template>

<script>
export default {
  name: 'Tema1',
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
