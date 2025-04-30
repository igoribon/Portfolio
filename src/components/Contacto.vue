<template>
  <section id="contacto" class="contact-section">
    <div class="section-header">
      <span class="section-number">05.</span>
      <h2>Contacto</h2>
    </div>

    <div class="contact-container">
      <div class="contact-content">
        <a href="mailto:igoribon@gmail.com" class="email-btn">
          Envíame un email
        </a>
      </div>

      <div class="social-links">
        <a href="https://linkedin.com/in/[tu-usuario]" target="_blank" rel="noopener noreferrer" title="LinkedIn">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg>
        </a>
        <a href="https://github.com/[tu-usuario]" target="_blank" rel="noopener noreferrer" title="GitHub">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
        </a>
        <a href="https://x.com/[tu-usuario]" target="_blank" rel="noopener noreferrer" title="X (Twitter)">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"></path></svg>
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
// No additional script needed
</script>

<style scoped>
.contact-section {
  padding: 100px 0;
  max-width: 800px;
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

.contact-container {
  padding: 0 2rem;
}

.contact-content {
  display: flex;
  justify-content: center;
  margin-bottom: 2rem;
}

.email-btn {
  display: inline-block;
  padding: 1rem 2rem;
  background: transparent;
  color: var(--primary-color);
  border: 1px solid var(--primary-color);
  border-radius: 4px;
  font-family: var(--font-mono);
  font-size: 1rem;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
}

.email-btn:hover {
  background: rgba(100, 255, 218, 0.1);
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 3rem;
}

.social-links a {
  color: var(--text-color);
  transition: color 0.3s ease;
}

.social-links a:hover {
  color: var(--primary-color);
}

.social-links svg {
  width: 24px;
  height: 24px;
}

@media (max-width: 768px) {
  .contact-container {
    padding: 0 1rem;
  }
}
</style>]]>