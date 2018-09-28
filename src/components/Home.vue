<template>
  <div class="home">
     
  <section class="hero">
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title">{{ heading }}</h1>
        <h2 class="subtitle">{{ subheading }}</h2>
      </div>
    </div>
  </section>

  <section class="servicios">
    <div class="container">
      <div class="columns is-desktop has-text-centered">
        
          <div class="column">
            <i class="fas fa-file-code "></i>
            <h2>{{ desarrollo }}</h2>
            <p><small class="parr">HTML / HTML5 + CSS / CSS3 + PHP/Laravel + jQuery / Javascript + Bootstrap + Photoshop / Illustrator + responsive / mobile + HTML email + Database / MySQL / SLQ Server</small></p>
          </div>
          <div class="column">
            <i class="fab fa-wordpress"></i>
            <h2>{{ cms }}</h2>
            <small class="parr">Diseño y personalización de temas de WordPress, Joomla y Drupal. Desarrollo de aplicaciones ajustadas a los requerimientos de cada sitio.</small>
          </div>
          <div class="column">
            <i class="fas fa-shopping-cart"></i>
            <h2>{{ ecom }}</h2>
            <small class="parr">WooCommerce + certificados + pasarelas de pago. Soluciones personalizadas para diferentes tipos de tiendas virtuales.</small>
          </div>

      </div>

     
          
      
    </div>
  </section>
  
  <section class="portfolio"></section>
  
  <section class="clientes"></section>
  
  <section class="formContacto"></section>

  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      heading: "¿Lorem ipsum dolor sit amet?",
      subheading:
        "Consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
      desarrollo: "BACKEND / FRONTEND",
      cms: "CONTENT MANAGER SYSTEM",
      ecom: "E-COMMERCE"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.hero
  background: url('../assets/clouds.jpg')
  background-size: cover

  .title
    +mobile
      font-weight: bold
    +tablet
      font-size: 2.5rem
    +desktop
      font-size: 4rem
      margin-top: 2rem

  h2
    margin: 1.5rem 0 2rem 0 !important

.servicios
  margin: 5rem 0 5rem 0 !important
  background-color: #gray

  .parr
    margin-top: 1.5rem

  .fa-shopping-cart
    font-size: 40px
    margin: 2rem 0 1.5rem 0 !important

  .fa-wordpress
    margin: 2rem 0 1.5rem 0 !important
    font-size: 40px

  .fa-file-code
    margin: 2rem 0 1.5rem 0 !important
    font-size: 40px

</style>
