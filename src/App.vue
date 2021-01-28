<template>
  <div class="antialiased bg-indigo-600">
    <Navbar />
    <HeroContent />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import HeroContent from "./components/HeroContent.vue";

export default {
  name: "App",
  components: {
    Navbar,
    HeroContent,
  },
};
</script>

<style>
</style>
