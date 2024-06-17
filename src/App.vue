<script setup lang="ts">
  import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <h1><RouterLink to="/">Inkh</RouterLink></h1>
      <nav>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/blog">Blog</RouterLink>
        <RouterLink to="/portfolio">Portfolio</RouterLink>
      </nav>
      <sub>Javascript Brute, Plushtoy Chiropractor, Cascading Stylish Sorceror</sub>
    </div>
  </header>

  <RouterView />
  <sub>6465047310 | code@inkh.io</sub>
</template>

<style scoped>
  sub { display: block; }

  @media ( min-width: 1024px ) {}
</style>
