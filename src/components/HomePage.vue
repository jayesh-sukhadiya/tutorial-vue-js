<template>
  <main class="home">
    <section class="hero">
      <div class="content">
        <h1>Build Vue Apps with Confidence</h1>
        <p>
          Follow this hands-on tutorial to learn the modern Vue 3 composition API,
          build reusable components, and ship polished interfaces faster.
        </p>
        <div class="actions">
          <button class="primary">Start Learning</button>
          <button class="secondary">View Docs</button>
        </div>
      </div>
      <div class="hero-card">
        <h2>Inside the Tutorial</h2>
        <ul>
          <li>Step-by-step lessons</li>
          <li>Real-world components</li>
          <li>Interactive projects</li>
        </ul>
      </div>
    </section>

    <section id="features" class="features">
      <article class="feature-card">
        <h3>Component Driven</h3>
        <p>Create composable UI building blocks and organize your code elegantly.</p>
      </article>
      <article class="feature-card">
        <h3>State Management</h3>
        <p>Learn best practices for managing app state with reactivity in mind.</p>
      </article>
      <article class="feature-card">
        <h3>Deploy Ready</h3>
        <p>Walk through real deployment workflows and performance optimizations.</p>
      </article>
    </section>

    <section id="tutorial" class="tutorial">
      <div class="tutorial-content">
        <h2>What You'll Build</h2>
        <p>
          Start from a blank canvas and end with a production-ready interface.
          Every chapter introduces new Vue concepts, from routing to state
          management, all applied in a practical, incremental way.
        </p>
      </div>
      <div class="tutorial-highlight">
        <h4>Next Lesson</h4>
        <p>Dynamic Components & Slots</p>
        <button class="primary">Continue</button>
      </div>
    </section>

    <section id="contact" class="cta-banner">
      <h2>Ready to dive in?</h2>
      <p>Join thousands of developers leveling up with Vue today.</p>
      <button class="primary">Join the Community</button>
    </section>
  </main>
</template>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  gap: 4rem;
  padding: 2rem 1.5rem 3rem;
  background: #f5f7fb;
  min-height: calc(100vh - 200px);
}

.hero {
  display: grid;
  grid-template-columns: minmax(0, 1.4fr) minmax(0, 1fr);
  gap: 2rem;
  align-items: center;
}

.content h1 {
  font-size: clamp(2.25rem, 5vw, 3.25rem);
  line-height: 1.1;
  margin-bottom: 1rem;
  color: #1e3c72;
}

.content p {
  color: #4f5464;
  font-size: 1.05rem;
  max-width: 540px;
  margin-bottom: 1.5rem;
}

.actions {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

button {
  border: none;
  border-radius: 999px;
  padding: 0.75rem 1.75rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

button.primary {
  background: linear-gradient(90deg, #1e3c72, #2a5298);
  color: #fff;
  box-shadow: 0 10px 24px rgba(30, 60, 114, 0.35);
}

button.secondary {
  background: #fff;
  color: #1e3c72;
  border: 1px solid rgba(30, 60, 114, 0.25);
}

button:hover,
button:focus {
  transform: translateY(-2px);
  box-shadow: 0 10px 24px rgba(30, 60, 114, 0.4);
}

.hero-card {
  background: #fff;
  border-radius: 20px;
  padding: 2rem;
  box-shadow: 0 18px 40px rgba(30, 60, 114, 0.15);
}

.hero-card h2 {
  margin-bottom: 1rem;
  color: #1e3c72;
}

.hero-card ul {
  list-style: none;
  display: grid;
  gap: 0.75rem;
  padding: 0;
  margin: 0;
}

.hero-card li::before {
  content: '✔';
  color: #2a5298;
  margin-right: 0.75rem;
}

.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 1.5rem;
}

.feature-card {
  background: #fff;
  border-radius: 16px;
  padding: 1.75rem;
  box-shadow: 0 12px 30px rgba(30, 60, 114, 0.12);
}

.feature-card h3 {
  margin-bottom: 0.75rem;
  color: #1e3c72;
}

.feature-card p {
  color: #4f5464;
}

.tutorial {
  display: grid;
  grid-template-columns: minmax(0, 1.5fr) minmax(0, 1fr);
  gap: 2rem;
  background: linear-gradient(120deg, rgba(30, 60, 114, 0.92), #2a5298);
  color: #fff;
  border-radius: 24px;
  padding: 3rem;
  box-shadow: 0 20px 42px rgba(30, 60, 114, 0.25);
}

.tutorial p {
  color: rgba(255, 255, 255, 0.85);
}

.tutorial-highlight {
  background: rgba(255, 255, 255, 0.08);
  border-radius: 20px;
  padding: 1.75rem;
  display: grid;
  gap: 0.75rem;
}

.tutorial-highlight button {
  justify-self: flex-start;
}

.cta-banner {
  text-align: center;
  background: #fff;
  border-radius: 24px;
  padding: 3rem 1.5rem;
  box-shadow: 0 18px 38px rgba(30, 60, 114, 0.18);
}

.cta-banner h2 {
  color: #1e3c72;
  margin-bottom: 0.75rem;
}

.cta-banner p {
  color: #4f5464;
  margin-bottom: 1.5rem;
}

@media (max-width: 1024px) {
  .hero,
  .tutorial {
    grid-template-columns: 1fr;
  }

  .tutorial {
    text-align: center;
  }

  .tutorial-highlight button {
    justify-self: center;
  }
}

@media (max-width: 600px) {
  .home {
    padding: 1.5rem 1rem 2.5rem;
  }

  .feature-card,
  .hero-card,
  .cta-banner,
  .tutorial {
    border-radius: 18px;
    padding: 1.75rem;
  }
}
</style>

