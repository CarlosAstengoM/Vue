<!-- Copyright(c) 2023, Carlos Astengo, All Rights Reserved -->
<script setup>
import { RouterLink, RouterView } from 'vue-router'
import TeamBanner from './components/TeamBanner.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <TeamBanner title="Branch Breakers Interactive" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/charts">Charts</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
