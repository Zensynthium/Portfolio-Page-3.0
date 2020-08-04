<template>
  <div>
    <particles class="fade-in">
    </particles>
    <cjumbo>
    </cjumbo>
  </div>
</template>

<script>
import cjumbo from '~/components/cJumbo.vue'
import particles from '~/components/Particles.vue'

export default {
  head: {
    title: 'A. Heggin Portfolio Page'
  },

  components: {
    cjumbo,
    particles
  },

}
</script>

}
<style>
/*
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
*/
html {
  animation: fade-in 0.3s ease-in;
}

hr {
  width: 50%;
  border-color: white;
}

.fade-in {
  animation: fade-in 0.3s ease-in;
}

@keyframes levitate {
  0% {top: 0px;}
  50% {top: 10px;}
  100% {top: 0px;}
}

@keyframes fade-in {
  from {opacity: 0;}
  to {opacity: 1;}
}
</style>
