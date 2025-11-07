<script setup>
import SiteHeader from './components/SiteHeader.vue'
import HomePage from './components/HomePage.vue'
import SiteFooter from './components/SiteFooter.vue'
</script>

<template>
  <div class="app-shell">
    <SiteHeader />
    <HomePage />
    <SiteFooter />
  </div>
</template>

<style scoped>
.app-shell {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  color: #1a1f36;
  background: #eef1f8;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>
