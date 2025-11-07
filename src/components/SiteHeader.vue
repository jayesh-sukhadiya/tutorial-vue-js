<template>
  <header class="site-header">
    <div class="container">
      <a class="brand" href="#">VueTutorial</a>
      <nav class="nav">
        <a class="nav-link" href="#features">Features</a>
        <a class="nav-link" href="#tutorial">Tutorial</a>
        <a class="nav-link" href="#contact">Contact</a>
      </nav>
      <button class="cta">Get Started</button>
    </div>
  </header>
</template>

<style scoped>
.site-header {
  position: sticky;
  top: 0;
  z-index: 100;
  background: linear-gradient(90deg, #1e3c72, #2a5298);
  color: #fff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
}

.container {
  max-width: 1120px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 1.5rem;
}

.brand {
  font-size: 1.25rem;
  font-weight: 700;
  color: inherit;
  text-decoration: none;
  letter-spacing: 0.05em;
}

.nav {
  display: flex;
  gap: 1.5rem;
}

.nav-link {
  color: rgba(255, 255, 255, 0.85);
  text-decoration: none;
  font-weight: 500;
  transition: color 0.2s ease;
}

.nav-link:hover,
.nav-link:focus {
  color: #fff;
}

.cta {
  border: none;
  border-radius: 999px;
  background: #fff;
  color: #1e3c72;
  font-weight: 600;
  padding: 0.5rem 1.5rem;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.cta:hover,
.cta:focus {
  transform: translateY(-1px);
  box-shadow: 0 6px 18px rgba(30, 60, 114, 0.35);
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
    gap: 1rem;
  }

  .nav {
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>

