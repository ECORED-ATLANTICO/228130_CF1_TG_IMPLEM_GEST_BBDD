<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

        
    p El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo:

    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="Bases de datos Las bases de datos son: SQL y NoSQL. 1. SQL: es un lenguaje de consulta estructurado. Los gestores son: ORACLE, SQL, Mysql y MariaDB. Sus características: a. Conformadas por tablas. b. Relacionales entre tablas. c. Solvencia y consistencia en el almacenamiento y consulta de datos. 2. NoSQL: es paradigma para la administración de BD. Los gestores son: MongoDB, Redis y Cassandra. Sus características son:  a. Los datos no se almacenan en tablas. b. Arquitectura distribuida. c. Eficiencia en el procesamiento de datos. d. Su almacenamiento se hace en documentos.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
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
