<template>
  <div id="app">
    <nav class="navbar has-shadow" role="navigation" aria-label="main navigation">
      <div class="container">
      
        <div class="navbar-brand">
          <a class="navbar-item r-item-logo" href="https://linkedin.com/in/jcguerra">
            Vue-CLI - JCGuerra
          </a>

          <span class="navbar-burger" v-on:click="toggleNav" v-bind:class="{ 'is-active': isActive }"> 
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </span>
        </div>

        <div class="navbar-menu" v-bind:class="{ 'is-active': isActive }">
          <div class="navbar-end">
            <router-link to="/" class="navbar-item r-item">Inicio</router-link>
            <router-link to="faq" class="navbar-item r-item">FAQ</router-link>

            <div class="navbar-item">
              <p class="control">
                <a class="button is-primary is-outlined" href="">
                  <span class="icon">
                    <i class="fas fa-envelope"></i>
                  </span>
                  <span> Contacto</span>
                </a>
              </p>
            </div>
          </div>
        </div>
   
      </div>
    </nav>
    
    <router-view/>


    <footer class="footer">
      <div class="container">
        
        <div class="level">

          <div class="level-left">
            <small>
              <a href="https://linkedin.com/in/jcguerra"><strong>JCGuerra</strong></a> 2018. Todos los derechos reservados.
            </small>
          </div>
          <div class="level-right">
            <span class="icon">
              <a class="" href="https://linkedin.com/in/jcguerra" target="_blank">
                <i class="fab fa-linkedin fa-2x"></i>
              </a>
            </span>
          </div>

        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function() {
    return {
      isActive: false
    };
  },
  methods: {
    toggleNav: function() {
      this.isActive = !this.isActive;
    }
  }
};
</script>

<style lang="sass">
@import '../node_modules/bulma/bulma.sass'
@import 'mq'

.navbar 
  background-color: #383838
  a:hover
    color: gray

.navbar-left a
a.r-item-logo
  color: #fff
  font-weigth: bold

a.r-item 
  color: #C1C1C1
  padding: 0.5rem 1.75rem
  +mobile
    &:hover
      background-color: #F1F1F1

.navbar-burger span
  background-color: #C1C1C1

footer
  a:link
    color: black
  a:hover
    color: gray


</style>
