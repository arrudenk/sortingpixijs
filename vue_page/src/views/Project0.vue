<template>
  <div class="project0">
    <h1>It's "Meteoroid"</h1>
    <div class="container">
      <iframe
          width="1210"
          height="600"
          :src="pixiProjectUrl"
          frameborder="0"
          allowfullscreen
      ></iframe>
    </div>
    <h2>This project is on
      <a href="https://github.com/arrudenk/Meteoroid_henocyd_1.24572552" target="_blank" rel="noopener">GitHub</a>.
    </h2>
    <h2> * My first js project made in 2 days to become Junior JS developer in NetEnt I needed some project to show, so I've created this masterpiece</h2>
    <h2> * Used some basic linear math algorithms here to show my understanding in this area</h2>
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

.container {
  position: relative;
}

.container iframe {
  width: 1210px; /* Original width */
  height: 600px; /* Original height */
  transform-origin: top left; /* Ensures the scaling starts from top left corner */
  transform: scale(0.5); /* Scales down the content to half its original size */
  border: 0;
  overflow: hidden; /* Ensures nothing goes outside the bounds of the iframe */
}

/* Container styling to fit the scaled iframe */
.container {
  width: 605px; /* New width */
  height: 300px; /* New height */
  overflow: hidden; /* Ensures that any overflow is hidden, which might not be necessary with the correct scaling */
  position: relative; /* Needed for absolute positioning inside */
}

/* Position the iframe absolutely within the .project0 container */
.container iframe {
  position: absolute;
  top: 0;
  left: 0;
}

@media (min-width: 1024px) {
  .project0 {
    min-height: 100vh;
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: center;
    align-content: center;
  }
}
</style>