<template>
  <section id="sobre-mi" class="about-section">
    <div class="section-header">
      <span class="section-number">02.</span>
      <h2>Sobre Mí</h2>
    </div>
    <div class="about-content">
      <div class="about-text">
        <p>
          ¡Hola! Mi nombre es Igor Aranguren y este es mi Portfolio.
        </p>

        <p>
          Mi interés por la informática nacío desde muy joven con aquellos primeros ordenadores de 8 bits. Posteriormente con mis estudios y mi trabajo diario esta faceta tuvo que quedar apartada. Durante los últimos 20 años he adquirido amplia experiencia en la gestión de proyectos y dirección de equipos multidisciplinares liderando iniciativas internacionales en sectores como el medioambiental y la logística. Pero desde hace un año decidí dar un giro a mi vida y centrarme en aquello que más me apasionaba. Me inscribí en un Bootcamp Full-Stak donde pude aprender todo lo relacionado con el desarrollo web.
        </p>
        <p>
          Avanzando rápidamente hasta hoy, he tenido el privilegio de trabajar en proyectos, tanto de desarrollo de mis capacidades a nivel académico como profesionales con la creación de páginas web. Mi enfoque principal estos días es construir productos accesibles e inclusivos y experiencias digitales. También me mantengo constantemente aprendiendo nuevas tecnologías y mejorando mis habilidades para mantenerme al día con las últimas tendencias.
        </p>

      <p >
        Destaco por mi capacidad para combinar la gestión eficiente de proyectos con el desarrollo de soluciones tecnológicas llave en mano, aportando expertise en comunicación con el cliente y trabajo en equipo
      </p>
      <a href="../assets/Currículum Igor Aranguren Full Stack.pdf" download class="cv-download">
        Descargar CV
      </a>
      </div>
      <div class="about-image">
        <div class="image-wrapper">
          <img src="../assets/images/igor.png" alt="foto de perfil" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.about-section {
  padding: 100px 0;
  max-width: 900px;
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

.about-content {
  display: grid;
  grid-template-columns: 3fr 2fr;
  gap: 50px;
  padding: 0 2rem;
}

.about-text p {
  color: var(--secondary-color);
  font-size: 1.1rem;
  line-height: 1.6;
  margin-bottom: 1rem;
}

.cv-download {
  display: inline-block;
  color: var(--primary-color);
  text-decoration: none;
  border: 1px solid var(--primary-color);
  border-radius: 4px;
  padding: 0.75rem 1rem;
  font-size: 1rem;
  transition: all 0.3s ease;
  margin-top: 1rem;
}

.cv-download:hover {
  background-color: var(--primary-color);
  color: var(--bg-color);
}

.image-wrapper {
  position: relative;
  max-width: 300px;
}

.image-wrapper::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 100%;
  border: 2px solid var(--primary-color);
  border-radius: 4px;
  top: 20px;
  left: 20px;
  z-index: -1;
}

.image-wrapper img {
  border-radius: 4px;
  filter: grayscale(100%) contrast(0.8);
  mix-blend-mode: normal;
  transition: all 0.3s ease;
}

.image-wrapper:hover img {
  filter: none;
  mix-blend-mode: normal;
}

@media (max-width: 768px) {
  .about-content {
    grid-template-columns: 1fr;
  }
  
  .image-wrapper {
    margin: 50px auto 0;
  }
}
</style>