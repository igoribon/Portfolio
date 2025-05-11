<template>
  <section id="skills" class="skills-section">
    <div class="section-header">
      <span class="section-number">03.</span>
      <h2>Mis Skills</h2>
    </div>
    <div class="skills-container">
      <div class="skill-category">
        <div class="skills-grid">
          <div class="skill-item">
            <h3>Frontend</h3>
            <ul class="skill-list">
              <li>HTML & CSS</li>
              <li>JavaScript (ES6+)</li>
              <li>Vue.js</li>
              <li>Responsive Design</li>
            </ul>
          </div>
          <div class="skill-item">
            <h3>Backend</h3>
            <ul class="skill-list">
              <li>Node.js</li>
              <li>Python</li>
              <li>SQL</li>
              <li>RESTful APIs</li>
            </ul>
          </div>
          <div class="skill-item">
            <h3>Herramientas</h3>
            <ul class="skill-list">
              <li>Git & GitHub</li>
              <li>VS Code</li>
              <li>Terminal</li>
              <li>Webpack/Vite</li>
              <li>Agile</li>
              <li>SCRUM</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.skills-section {
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

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  padding: 0 2rem;
}

.skill-item {
  background: rgba(255, 255, 255, 0.05);
  padding: 2rem;
  border-radius: 4px;
  transition: transform 0.3s ease;
}

.skill-item:hover {
  transform: translateY(-5px);
}

h3 {
  color: var(--primary-color);
  font-family: var(--font-mono);
  font-size: 1.2rem;
  margin-bottom: 1.5rem;
}

.skill-list {
  list-style: none;
}

.skill-list li {
  color: var(--secondary-color);
  margin-bottom: 0.8rem;
  position: relative;
  padding-left: 1.2rem;
}

.skill-list li::before {
  content: "▹";
  position: absolute;
  left: 0;
  color: var(--primary-color);
}
</style>