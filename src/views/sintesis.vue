<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p Este componente formativo aborda de manera integral el patronaje infantil de prendas deportivas, iniciando con la interpretación y trazado de tipologías básicas como camiseta, camisilla, sudadera de punto y mallas. A partir de estos fundamentos, se introduce el proceso de escalado de prendas de vestir, comprendiendo su concepto, objetivos y principios técnicos. Asimismo, se exploran los diferentes tipos de escalado, incluyendo el proporcional, combinado y diferencial, junto con la aplicación práctica de métodos como el básico, monobásico y por coordenadas. Finalmente, se orienta al aprendiz en la separación de tallas y la correcta marcación de patrones, fortaleciendo así competencias clave para su aplicación en contextos productivos de la industria de la confección. 
    

    .row.justify-content-center
      .col-lg-10.mb-5.bgs.p-4.brad
        figure
          img(src="@/assets/curso/sintesis.svg", alt="Descripción imagen")
      .col-auto
        a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/bullets/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
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
