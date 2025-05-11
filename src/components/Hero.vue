<template>
  <section class="hero" id="inicio">
    <div class="hero-content">
      <p class="greeting">Hola, mi nombre es</p>
      <h1 class="name">Igor Aranguren.</h1>
      <h2 class="title">Desarrollo de soluciones digitales.</h2>
      <p class="description">
        Soy un desarrollador full-stack web especializado en crear apps digitales para la solución de las necesidades. 
        Actualmente, me enfoco en construir productos accesibles y centrados en el usuario utilizando todas las herramientas a mi disposición.
        Me apasiona aprender nuevas tecnologías y mejorar mis habilidades para ofrecer soluciones innovadoras y efectivas.
      </p>
      <div class="cta-buttons">
        <a href="#proyectos" class="btn primary">Ver mi trabajo</a>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  padding: 0 2rem;
  margin-top: -80px; /* Compensar el header fijo */
}

.hero-content {
  max-width: 1000px;
  margin: 0 auto;
}

.greeting {
  font-family: var(--font-mono);
  color: var(--primary-color);
  font-size: 1rem;
  margin-bottom: 1.5rem;
}

.name {
  font-size: clamp(40px, 8vw, 80px);
  font-weight: bold;
  line-height: 1.1;
  margin: 0;
  color: var(--text-color);
}

.title {
  font-size: clamp(40px, 8vw, 80px);
  font-weight: bold;
  line-height: 1.1;
  margin: 0.3em 0 1em;
  color: var(--secondary-color);
}

.description {
  max-width: 540px;
  margin-bottom: 3rem;
  color: var(--secondary-color);
  font-size: 1.2rem;
  line-height: 1.6;
}

.btn {
  display: inline-block;
  padding: 1.25rem 1.75rem;
  border: 1px solid var(--primary-color);
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 0.9rem;
  line-height: 1;
  text-decoration: none;
  cursor: pointer;
  transition: all 0.25s cubic-bezier(0.645,0.045,0.355,1);
  margin-top: 1rem;
}

.btn.primary {
  background-color: transparent;
  color: var(--primary-color);
}

.btn.primary:hover {
  background-color: rgba(100,255,218,0.1);
}
</style>