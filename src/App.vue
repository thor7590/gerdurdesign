<template>
  <v-app>
      <portfolio-header></portfolio-header>
      <portfolio-nav></portfolio-nav>
      <v-content>
        <router-view></router-view>
      </v-content>
      <portfolio-footer></portfolio-footer>
  </v-app>  
</template>

<script>
import header from './views/header.vue'
import nav from './views/nav.vue'
import footer from './views/footer'


export default {
  name: 'App',

 components: {
   'portfolio-header':header,
   'portfolio-nav':nav,
   'portfolio-footer':footer
 },
 
  data: () => ({
    //
  })
}
</script>

<style lang="scss">
  nav {
 
  padding: 30px;
  a {
    
    color: #222222 !important;
    &.router-link-exact-active {
      color: #8f8f8f !important;
      font-weight: bold;
    }
  }
}
</style>