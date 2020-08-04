<template>
  <div class="jumbotron custom-jumbo text-center">
    <h1 class="display-4">Anthony Heggin</h1>
    <h2 class="lead">Creating the next generation of Web Applications</h2>
    <div>
      <b-button class="raise-up" href="#projects" variant="dark">Discover More</b-button>
      <b-button class="raise-up" href="#contact" variant="outline-secondary">Contact Me</b-button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'cjumbo',
    data () {
    return {
    }
  }
}
</script>

<style>
.custom-jumbo {
  background-image: linear-gradient(to bottom, rgba(0,0,0,0.5), rgba(255, 255, 255, 1));
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  place-items: center;
  height: calc(100vh - 56px);
  text-shadow: 1px 1px 2px #888;
  margin: 0;
  border-radius: 0;
}

.raise-up {
  position: relative;
  top: 20px;
  z-index: 1;
}

html {
font-size: 1rem;
}

@include media-breakpoint-up(sm) {
html {
font-size: 1.2rem;
}
}

@include media-breakpoint-up(md) {
html {
font-size: 1.4rem;
}
}

@include media-breakpoint-up(lg) {
html {
font-size: 1.6rem;
}
}
</style>