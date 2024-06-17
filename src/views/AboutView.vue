<template>
  <h1>{{ headerLit }}</h1>
  <div class="rant">
    <p v-for="lit in aboutLit">{{ lit }}</p>
  </div>
</template>

<script setup lang="ts">
  const headerLit = `About Me`
  const aboutLit = `
    As an impassioned engineer, I started my focus on core technologies
    I want to know how things work and why they were done that way
    But that knowledge is infinite and I am very finite
    Now I'm focused soley on what I can create and what I need to create it
    A Pragmatic Engineer
    I personally care about creating something new and not chasing after trends
    Fulfilling needs that exist instead of trying to create new demands
    I've learned business and management the same way I learned to code
    From my environment, as necessary
    What I seek now is a role in which I can truly flourish and be challenged
    A place to take root
  `.trim().split( /\s*\n\s*/g )
</script>