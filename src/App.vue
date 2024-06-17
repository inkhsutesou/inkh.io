<script setup lang="ts">
  import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <h1><RouterLink to="/">Inkh-Su Tesou</RouterLink></h1>
      <nav>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/portfolio">Portfolio</RouterLink>
      </nav>
      <sub>Javascript Brute, Plushtoy Chiropractor, Cascading Stylish Sorceror</sub>
    </div>
  </header>

  <RouterView />
  <sub><a href="tel:6465047310">6465047310</a> | <a href="mailto:code@inkh.io">code@inkh.io</a></sub>
</template>

<style scoped>
  sub { display: block; }

  @media ( min-width: 1024px ) {}
</style>
