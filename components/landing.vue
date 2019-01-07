<template>
  <div id="landing">
    <h1 id="title">Movie Compass</h1>
    <p id="message">Find your way to a nearby movie</p>

    <form id="location-input">
      <input placeholder="Please enter your location.">
      <hr>
      <button id="location-find">Find your location</button>
    </form>
  </div>
</template>

<script>
export default {

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

div form {
  padding-top: 15rem;
}

div form input,button {
  text-align: center;
  width: 15rem;
}

</style>
