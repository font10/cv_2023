<template>
  <div class="container-fluid p-0 m-0">
    <Hero />
    <About />
    <Servicios />
    <Portfolio />
    <Estudios />
    <Trabajo />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/Hero.vue'
import About from '@/components/About.vue'
import Servicios from '@/components/Servicios.vue'
import Portfolio from '@/components/Portfolio.vue'
import Estudios from '@/components/Estudios.vue'
import Trabajo from '@/components/Trabajo.vue'
import Contact from '@/components/Contact.vue'

export default {
  name: 'HomeView',
  components: {
    Hero,
    About,
    Servicios,
    Portfolio,
    Estudios,
    Trabajo,
    Contact
  }
}
</script>

<style scoped>
.container.fluid {
  
  background-color: #02061a;
}
</style>
