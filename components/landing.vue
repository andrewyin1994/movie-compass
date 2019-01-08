<template>
  <div id="landing">
    <h1 id="title">Movie Compass</h1>
    <p id="message">Find your way to a nearby movie</p>

    <section id="location-form">
      <input placeholder="Please enter your location.">
      <hr>
      <button
        id="location-find"
        @click="findCoords">Find your location
      </button>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      lat: 0,
      long: 0
    }
  },
  methods: {
    findCoords() {
      if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(
          pos => {
            this.lat = pos.coords.latitude;
            this.long = pos.coords.longitude;
            alert(
              `Latitude: ${this.lat}`
              + `\nLongitude: ${this.long}`);
          },
          () => {
            alert("Could not find location.");
          }
        );
      }
    }
  }
}
</script>

<style>
div {
  display: flex;
  flex-direction: column;
  text-align: center;
}

div h1 {
  padding-top: 10rem;
}

div p {
  padding-top: 1rem;
}

div #location-form {
  padding-top: 15rem;
}

div #location-form input,button {
  text-align: center;
  width: 15rem;
}

</style>
