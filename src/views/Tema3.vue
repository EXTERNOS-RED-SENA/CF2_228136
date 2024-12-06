<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 3
      h1 Análisis exploratorio de datos
    
    .bloque-texto-g.color-secundario.p-3.p-sm-4.p-md-5(data-aos="flip-up" data-aos-duration="1000")
      .bloque-texto-g__img(
        :style="{'background-image': `url(${require('@/assets/curso/tema3/1.png')})`}"
      )
      .bloque-texto-g__texto.p-4
        p.mb-0 El análisis exploratorio de datos (EDA, por sus siglas en inglés) constituye una etapa fundamental en el proceso de comprensión y preparación de datos para modelos de inteligencia artificial. Esta fase inicial de investigación ayuda a los analistas a comprender las características fundamentales de los conjuntos de datos, identificar patrones significativos y detectar anomalías que podrían afectar análisis posteriores. A diferencia de los métodos estadísticos confirmatorios, el EDA adopta un enfoque más flexible y orientado al descubrimiento, permitiendo que los datos revelen sus secretos de manera orgánica.
      
    Separador

    .titulo-segundo(data-aos="flip-up")
      h2#t_3_1 3.1 Estadística descriptiva e inferencial
    
    p(data-aos="fade-up") La estadística descriptiva proporciona el conjunto de herramientas fundamental para comenzar cualquier análisis exploratorio. A través de medidas de tendencia central, dispersión y forma, los analistas pueden obtener una primera aproximación a la naturaleza de sus datos. Sin embargo, el verdadero poder de la estadística descriptiva radica en su capacidad para revelar aspectos sutiles de los datos que podrían pasar desapercibidos en un examen superficial.

    .row.mt-4
      .col-lg-auto.d-none.d-lg-block(data-aos="fade-right")
        figure
          img(src="@/assets/curso/tema3/2.png")
      .col-lg(data-aos="fade-left")
        .p-4(style="background-color:#ECF2FF;")
          .row
            .col-md-auto.d-none.d-md-block
              figure
                img(src="@/assets/curso/tema3/3.svg")
            .col-md
              p.mb-0 Las medidas de tendencia central, como la media, mediana y moda, ofrecen diferentes perspectivas sobre el centro de los datos. Por ejemplo, en distribuciones altamente sesgadas, la diferencia significativa entre la media y la mediana puede revelar la presencia de valores extremos que requieren atención especial. La dispersión de los datos, medida a través de la varianza, desviación estándar y rango intercuartílico, proporciona información clave sobre la variabilidad y la confiabilidad de las mediciones.
        p.mt-4.mb-0 Por su parte, la estadística inferencial permite extender las conclusiones obtenidas de una muestra a la población general. Este proceso requiere una comprensión profunda de conceptos como intervalos de confianza, pruebas de hipótesis y significancia estadística. En el contexto del análisis exploratorio, las técnicas inferenciales ayudan a validar patrones observados y a determinar si las relaciones descubiertas son estadísticamente significativas.
    
    Separador

    .titulo-segundo(data-aos="flip-up")
      h2#t_3_2 3.2 Métodos de análisis univariable y multivariable
    .row.mt-4
      .col-lg(data-aos="fade-right")
        p.mb-4 El análisis univariable representa el primer paso en la exploración detallada de cada variable individual dentro de un conjunto de datos. Este análisis fundamental examina la distribución, centralidad, dispersión y forma de cada variable por separado, proporcionando una base sólida para análisis más complejos. Los principales aspectos que se deben considerar en el análisis univariable incluyen:
        .p-4.mt-4.mb-4(style="background-color:#ECF2FF;")
          ol.lista-ol--cuadro.mb-0
            li.d-flex
              .lista-ol--cuadro__vineta
                span.fw-bold 1
              span Distribución de frecuencias y visualizaciones básicas.
            li.d-flex
              .lista-ol--cuadro__vineta
                span.fw-bold 2
              span Detección de valores atípicos y anomalías.
            li.d-flex
              .lista-ol--cuadro__vineta
                span.fw-bold 3
              span Análisis de valores faltantes.
            li.d-flex
              .lista-ol--cuadro__vineta
                span.fw-bold 4
              span Evaluación de la normalidad.
            li.d-flex.mb-0
              .lista-ol--cuadro__vineta
                span.fw-bold 5
              span Identificación de patrones temporales o secuenciales
        p.mb-0 El análisis multivariable, por su parte, examina las relaciones entre múltiples variables simultáneamente. Este enfoque es particularmente relevante en el contexto de la inteligencia artificial, donde los modelos frecuentemente deben procesar numerosas variables interrelacionadas. #[strong La complejidad de estas relaciones puede apreciarse mejor a través de la siguiente tabla comparativa:]
      .col-lg-auto.d-none.d-lg-block(data-aos="fade-left")
        figure
          img(src="@/assets/curso/tema3/4.png")
    
    .titulo-sexto.color-acento-contenido.mt-4(data-aos="fade-down")
      h5 Tabla 2.
      span Tipos de análisis: técnicas, aplicaciones y consideraciones clave
    .tabla-a.color-acento-contenido(data-aos="fade-up")
      table
        caption.fw-normal #[strong Fuente.] OIT, 2024.
        thead
          tr.text-white.text-center(style="background-color:#03A9F4;")
            th Tipo de Análisis.
            th Técnicas Principales.
            th Aplicaciones.
            th Consideraciones clave.
        tbody.text-center
          tr.bg-white
            td Bivariado.
            td Correlación de Pearson, Chi-cuadrado.
            td Relaciones entre pares de variables.
            td Asunciones de linealidad.
          tr.bg-white
            td Regresión múltiple.
            td Mínimos cuadrados, Ridge, Lasso.
            td Predicción de variables continuas.
            td Multicolinealidad.
          tr.bg-white
            td Análisis factorial.
            td PCA, Factor Analysis.
            td Reducción de dimensionalidad.
            td Interpretabilidad de factores.
          tr.bg-white
            td Análisis de clústeres.
            td K-means, jerárquico.
            td Segmentación de datos.
            td Selección de número de grupos.
          tr.bg-white
            td Análisis discriminante.
            td LDA, QDA.
            td Clasificación supervisada.
            td Separabilidad de clases.
    
    Separador

    .titulo-segundo(data-aos="flip-up")
      h2#t_3_3 3.3 Técnicas de visualización
    
    p(data-aos="fade-up") La visualización de datos representa una herramienta indispensable en el análisis exploratorio, transformando números abstractos en representaciones visuales intuitivas que facilitan la identificación de patrones, tendencias y anomalías. Las técnicas de visualización modernas van más allá de los gráficos básicos, incorporando elementos interactivos y múltiples dimensiones de información en una sola representación.

    .row.mt-4
      .col-lg-auto.d-none.d-lg-block(data-aos="fade-right")
        figure
          img(src="@/assets/curso/tema3/5.png")
      .col-lg(data-aos="fade-left")
        .p-4(style="background-color:#F7EEFE;")
          .row
            .col-md-auto.d-none.d-md-block
              figure
                img(src="@/assets/curso/tema3/6.svg")
            .col-md
              p.mb-0 La selección de la técnica de visualización adecuada depende tanto de la naturaleza de los datos como del objetivo del análisis. Por ejemplo, los diagramas de dispersión resultan invaluables para examinar relaciones entre variables continuas, mientras que los gráficos de calor pueden revelar patrones complejos en matrices de correlación. Los gráficos de caja (#[b box plots]) combinan múltiples aspectos de la distribución de datos, mostrando simultáneamente la mediana, cuartiles y valores atípicos.
      p.mt-4.mb-0 En el contexto del #[b big data] y la inteligencia artificial, las técnicas de visualización han evolucionado para manejar volúmenes masivos de datos. Las visualizaciones interactivas permiten a los analistas explorar diferentes niveles de detalle, mientras que las técnicas de reducción de dimensionalidad como t-SNE y UMAP facilitan la visualización de datos altamente dimensionales en espacios bidimensionales o tridimensionales.
    
    .row.mt-4
      .col-lg(data-aos="fade-right")
        p La efectividad de una visualización no solo depende de su precisión técnica, sino también de su capacidad para comunicar información de manera clara y convincente. Los principios de diseño visual, como el uso apropiado del color, la gestión del espacio y la jerarquía visual, desempeñan un papel destacado en la creación de visualizaciones que sean tanto informativas como accesibles
        p.mb-0.fw-bold El análisis exploratorio de datos, con sus múltiples facetas y técnicas, es una fase crítica en cualquier proyecto de análisis de datos o inteligencia artificial. La combinación de estadística rigurosa, análisis multivariable y visualización efectiva proporciona los cimientos necesarios para construcción de modelos robustos y confiables.
      .col-lg-auto.d-none.d-lg-block(data-aos="fade-left")
        figure
          img(src="@/assets/curso/tema3/7.png")



</template>

<script>
import LineaTiempoD from '../bootstrap/LineaTiempoD.vue'
export default {
  name: 'Tema3',
  components: {
    LineaTiempoD,
  },
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
