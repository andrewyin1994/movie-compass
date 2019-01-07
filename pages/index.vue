<template>
  <section class="container">
    <!-- <Geolocation /> -->
    <Landing />
  </section>
</template>

<script>
// import Geolocation from "../components/Geolocation.vue";
import Landing from "../components/landing.vue";

export default {
  layout: "home-layout",
  components: {
    Landing
    // Geolocation
  }
};
</script>

<style>
</style>
