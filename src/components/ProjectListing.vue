<script setup lang="ts">
defineProps({ item: {} })
</script>

<template>
  <h1>{{ item.company }}</h1>
  <h3>{{ item.title }}</h3>
  <ul>
    <li v-for="info in item.description.trim().split(/\s*\n\s*/g)">
      {{ info }}
    </li>
  </ul>
  <div class="image-container" :data-length="item.images.length">
    <img v-for="src in item.images" :src="src" />
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
}

h3 {
  font-size: 1.2rem;
}

.image-container {
  font-size: 0;
}
.image-container img {
  vertical-align: top;
}
.image-container[ data-length = "4" ] img {
  width: 50%;
  max-height: 50%;
}
.image-container[ data-length = "3" ] img {
  width: 50%;
  max-height: 50%;
}
.image-container[ data-length = "3" ] img:nth-child( 2 ) {
  width: 100%;
}
.image-container[ data-length = "2" ] img {
  width: 50%;
}
.image-container[ data-length = "1" ] img {
  width: 100%;
}
</style>
