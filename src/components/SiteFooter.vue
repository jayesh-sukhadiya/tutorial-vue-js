<template>
  <footer class="site-footer">
    <div class="container">
      <div class="brand">
        <strong>VueTutorial</strong>
        <p>Built with Vue 3 and a passion for teaching modern web development.</p>
      </div>
      <div class="links">
        <a href="#features">Features</a>
        <a href="#tutorial">Tutorial</a>
        <a href="#contact">Support</a>
      </div>
      <div class="copyright">
        <p>&copy; {{ new Date().getFullYear() }} VueTutorial. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.site-footer {
  background: #101633;
  color: rgba(255, 255, 255, 0.82);
  padding: 2.5rem 1.5rem;
}

.container {
  max-width: 1120px;
  margin: 0 auto;
  display: grid;
  gap: 2rem;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  align-items: start;
}

.brand strong {
  font-size: 1.15rem;
  display: block;
  margin-bottom: 0.5rem;
}

.brand p {
  margin: 0;
  color: rgba(255, 255, 255, 0.65);
}

.links {
  display: grid;
  gap: 0.75rem;
}

.links a {
  color: rgba(255, 255, 255, 0.78);
  text-decoration: none;
  transition: color 0.2s ease;
}

.links a:hover,
.links a:focus {
  color: #fff;
}

.copyright {
  color: rgba(255, 255, 255, 0.6);
  font-size: 0.9rem;
}
</style>

