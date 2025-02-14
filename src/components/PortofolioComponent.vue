<template>
  <div class="portfolio-container">
    <div class="grid-layout">
      <!-- Top Left - Arrow -->
      <div class="arrow-section">
        <div class="circle">
          <span class="arrow">→</span>
        </div>
      </div>

      <!-- Top Right - Name and Title -->
      <div class="info-section">
        <h1 class="name">Perdana Faishal M</h1>
        <p class="title">Software Engineer | Frontend Engineer | Fullstack Engineer</p>
      </div>

      <!-- Bottom Left - Large Text -->
      <div class="large-text-section">
        <h2>Software<br>Engineer</h2>
      </div>

      <!-- Bottom Right - Contact Links -->
      <div class="contact-section">
        <div class="link-item">
          <span class="icon">📞</span>
          <a href="#portfolio">Go to Portfolio</a>
        </div>
        <div class="link-item">
          <span class="icon">🏠</span>
          <a href="#portfolio">Go to Portfolio</a>
        </div>
        <div class="link-item">
          <span class="icon">✉️</span>
          <a href="mailto:meetfaishal@gmail.com">meetfaishal@gmail.com</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'PortfolioHeader'
}
</script>

<style scoped>
.portfolio-container {
  background-image: url('../assets/waves.svg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  border: 1px #555555 solid;
  border-radius: 24px;
  max-height: 100vh;
  padding: 2rem;
  font-family: system-ui, -apple-system, sans-serif;
}

.grid-layout {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  gap: 2rem;
  max-width: 1400px;
  margin: 0 auto;
}

/* Top Left */
.arrow-section {
  display: flex;
  align-items: flex-start;
}

.circle {
  width: 48px;
  height: 48px;
  border: 2px solid #000;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.arrow {
  font-size: 1.5rem;
}

/* Top Right */
.info-section {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
}

.name {
  font-size: 3.5rem;
  font-weight: 700;
  margin: 0;
  margin-bottom: 0.5rem;
}

.title {
  font-size: 1.25rem;
  color: #555;
  margin: 0;
}

/* Bottom Left */
.large-text-section {
  display: flex;
  align-items: flex-end;
}

.large-text-section h2 {
  font-size: 5rem;
  font-weight: 900;
  line-height: 1;
  margin: 0;
}

/* Bottom Right */
.contact-section {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  gap: 1.5rem;
}

.link-item {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.icon {
  font-size: 1.5rem;
}

a {
  color: #000;
  text-decoration: none;
  font-size: 1.25rem;
}

a:hover {
  text-decoration: underline;
}

@media (max-width: 1024px) {
  .name {
    font-size: 2.5rem;
  }

  .large-text-section h2 {
    font-size: 4rem;
  }
}

@media (max-width: 768px) {
  .grid-layout {
    grid-template-columns: 1fr;
    grid-template-rows: auto;
  }

  .large-text-section h2 {
    font-size: 3rem;
  }

  .name {
    font-size: 2rem;
  }

  .contact-section {
    justify-content: flex-start;
  }
}
</style>
