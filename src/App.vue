<template>
  <div class="app">
    <Header />
    <main>
      <Hero />
      <About />
      <Skills />
      <Projects />
      <Contacto />
    </main>
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Contacto from './components/Contacto.vue'

</script>

<style>
.app {
  min-height: 100vh;
}

main {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}
</style>
