<script setup lang="ts">
import NavBar from './components/NavBar.vue';
import Hero from './components/Hero.vue';
import Fotter from './components/Fotter.vue';
</script>

<template>

  <div id="app" class="min-h-screen relative overflow-hidden">
    <img src="../src/assets/hero-desktop.png" class="hidden md:block absolute inset-0 w-full h-full object-cover -z-10" alt="delicious-food"/>
    <img src="../src/assets/hero-mobile.png" class="md:hidden absolute inset-0 w-full h-full object-cover -z-10" alt="delicious-food"/>
    <div  class=" max-w-7xl mx-auto p-6 md:p-6">
      <NavBar/>
      <Hero/>
      <Fotter/>
    </div>
  </div>
</template>
