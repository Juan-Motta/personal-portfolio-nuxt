<template>
  <div class="container mx-auto">
    <Navbar />
    <Hero />
    <section class="stars-container">
      <div class="star-backgroud-1"></div>
      <div class="star-backgroud-2"></div>
      <div class="star-backgroud-3"></div>
    </section>
  </div>
</template>

<script setup>
const colorMode = useColorMode();

console.log(colorMode.preference);
</script>
