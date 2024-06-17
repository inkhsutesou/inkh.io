<script setup lang="ts">
defineProps({ item: {} })
</script>

<template>
  <h1>{{ item.company }}</h1>
  <sub>{{ item.title }}</sub>
  <ul>
    <li v-for="info in item.description.trim().split(/\s*\n\s*/g)">
      {{ info }}
    </li>
  </ul>
  <div class="image-container">
    <img v-for="src in item.images" :src="src" />
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
