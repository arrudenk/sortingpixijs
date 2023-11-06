<template>
  <div class="project0">
    <h1>This PIXI JS representation</h1>
    <iframe
        width="1280"
        height="720"
        :src="pixiProjectUrl"
        frameborder="0"
        allowfullscreen
    ></iframe>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pixiProjectUrl: 'https://arrudenk.github.io/Meteoroid_henocyd_1.24572552/'
    };
  }
};
</script>

<style>
@media (min-width: 1024px) {
  .project0 {
    min-height: 100vh;
    align-items: center;
  }
}
</style>