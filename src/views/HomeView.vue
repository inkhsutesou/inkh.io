<template>
  <h1>{{ headerLit }}</h1>
  <div class="rant">
    <p v-for="lit in rantLit">{{ lit }}</p>
  </div>
</template>

<script setup lang="ts">
  const headerLit = `Hello, I'm Inkh`
  const rantLit = `
    I've been around since Javascript was unpopular;
    When it wasn't a " real " programming language;
    I remember an internet without rounded corners;
    XSS practices existed because of coders like me;
    I said Coffeescript was dumb and now it's dead;
    I prayed for CSS vars then, and I pray for native CSS nesting now;
    I watched jQuery, MooTools, Backbone, Ember rise and fall;
    and I'll write JavaScript well after some blogger writes " Is React.js dead ? ";
    I'll be writing Javascript when AI has Javascript perfected;
    ;
    I have strong feelings about it.  Hire me;
  `.trim().split( /\s*\n\s*/g )
</script>

<style>
  .rant {
    font-size: 1.5rem;
    width: 70%;
  }
</style>