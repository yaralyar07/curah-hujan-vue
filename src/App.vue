<template>
  <div class="min-h-screen flex flex-col">
    <Navbar />
    
    <HeroSection />
  </div>
</template>

<script setup>
import Navbar from './components/Navbar.vue';
import HeroSection from './components/HeroSection.vue';
</script>

<style>
/* Reset dasar jika diperlukan */
body {
  margin: 0;
  padding: 0;
}
</style>