<template>
  <header class="header">
    <nav class="nav-container">
      <div class="logo">
        <a href="#inicio">IB</a>
      </div>
      <ul class="nav-links">
        <li><a href="#inicio"><span>01.</span> Inicio</a></li>
        <li><a href="#sobre-mi"><span>02.</span> Sobre Mí</a></li>
        <li><a href="#skills"><span>03.</span> Skills</a></li>
        <li><a href="#proyectos"><span>04.</span> Proyectos</a></li>
        <li><a href="#contacto"><span>05.</span> Contacto</a></li>
      </ul>
    </nav>
  </header>
</template>

<script setup>
</script>

<style scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  background-color: rgba(21, 21, 21, 0.95);
  backdrop-filter: blur(10px);
  padding: 1rem 2rem;
}

.nav-container {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo a {
  font-family: var(--font-mono);
  font-size: 1.5rem;
  font-weight: bold;
  color: var(--primary-color);
}

.nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
}

.nav-links a {
  color: var(--text-color);
  text-decoration: none;
  font-family: var(--font-mono);
  font-size: 0.9rem;
  transition: color 0.3s ease;
}

.nav-links span {
  color: var(--primary-color);
  font-size: 0.8rem;
  margin-right: 0.5rem;
}

.nav-links a:hover {
  color: var(--primary-color);
}
</style>