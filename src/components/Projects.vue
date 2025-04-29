<template>
  <section id="proyectos" class="projects-section">
    <div class="section-header">
      <span class="section-number">04.</span>
      <h2>Proyectos Destacados</h2>
    </div>
    <div class="projects-grid">
      <article class="project-card">
        <div class="project-content">
          <div class="project-overline">Proyecto Destacado</div>
          <h3 class="project-title">
            <a href="#" target="_blank" rel="noopener noreferrer">Título del Proyecto</a>
          </h3>
          <div class="project-description">
            <p>
              Una breve descripción del proyecto destacando las características principales
              y el impacto del mismo. Explica qué problema resuelve y qué tecnologías
              utilizaste para desarrollarlo.
            </p>
          </div>
          <ul class="project-tech-list">
            <li>Vue.js</li>
            <li>Node.js</li>
            <li>MongoDB</li>
          </ul>
          <div class="project-links">
            <a href="#" target="_blank" rel="noopener noreferrer" aria-label="GitHub Link">
              <svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-github"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
            </a>
            <a href="#" target="_blank" rel="noopener noreferrer" aria-label="External Link">
              <svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-external-link"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path><polyline points="15 3 21 3 21 9"></polyline><line x1="10" y1="14" x2="21" y2="3"></line></svg>
            </a>
          </div>
        </div>
        <div class="project-image">
          <img src="project-image.jpg" alt="Screenshot del proyecto" />
        </div>
      </article>
      
      <!-- Puedes duplicar el article.project-card para más proyectos -->
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.projects-section {
  padding: 100px 0;
  max-width: 1000px;
  margin: 0 auto;
}

.section-header {
  display: flex;
  align-items: center;
  margin-bottom: 3rem;
  gap: 1rem;
}

.section-number {
  color: var(--primary-color);
  font-family: var(--font-mono);
  font-size: 1.2rem;
}

h2 {
  font-size: 2rem;
  color: var(--text-color);
}

.project-card {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  align-items: center;
  margin-bottom: 100px;
}

.project-content {
  position: relative;
  grid-area: 1 / 1 / -1 / 7;
  grid-column: 1 / 8;
  z-index: 2;
}

.project-image {
  grid-area: 1 / 6 / -1 / -1;
  position: relative;
  z-index: 1;
}

.project-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 4px;
  filter: grayscale(100%) contrast(1);
  transition: all 0.3s ease;
}

.project-image:hover img {
  filter: none;
}

.project-overline {
  margin: 10px 0;
  color: var(--primary-color);
  font-family: var(--font-mono);
  font-size: 0.9rem;
}

.project-title {
  margin: 0 0 20px;
  font-size: 2rem;
}

.project-title a {
  color: var(--text-color);
  text-decoration: none;
}

.project-description {
  padding: 25px;
  background-color: rgba(255, 255, 255, 0.05);
  color: var(--secondary-color);
  border-radius: 4px;
  font-size: 1rem;
  line-height: 1.6;
}

.project-tech-list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  padding: 0;
  margin: 25px 0 10px;
  list-style: none;
}

.project-tech-list li {
  color: var(--secondary-color);
  font-family: var(--font-mono);
  font-size: 0.9rem;
}

.project-links {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-top: 1rem;
}

.project-links a {
  color: var(--text-color);
  transition: color 0.3s ease;
}

.project-links a:hover {
  color: var(--primary-color);
}

.project-links svg {
  width: 20px;
  height: 20px;
}

@media (max-width: 768px) {
  .project-card {
    grid-template-columns: 1fr;
  }

  .project-content {
    grid-column: 1 / -1;
    padding: 40px 40px 30px;
    text-align: left;
  }

  .project-image {
    grid-column: 1 / -1;
    opacity: 0.25;
  }
}
</style>