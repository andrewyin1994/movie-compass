<template>
  <section class="container-fluid">
    <Poster/>
    <div style="height: 1000px"/>
  </section>
</template>

<script>
import Poster from '../components/Poster.vue';

export default {
  layout: "home-layout",
  components: {
    Poster
  }
};
</script>

<style lang="scss">
</style>
