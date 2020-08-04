<template>
<client-only>
  <Particles
      id="tsparticles"
      :options="{
            background: {
                color: {
                    value: ''
                }
            },
            fpsLimit: 60,
            interactivity: {
                detectsOn: 'canvas',
                events: {
                    onClick: {
                        enable: false,
                        mode: 'bubble'
                    },
                    onHover: {
                        enable: true,
                        mode: 'bubble'
                    },
                    resize: true
                },
                modes: {
                    bubble: {
                        distance: 100,
                        duration: 0.2,
                        opacity: 0.8,
                        size: 10,
                        speed: 3
                    },
                    push: {
                        quantity: 4
                    },
                    repulse: {
                        distance: 50,
                        duration: 0.2
                    }
                }
            },
            particles: {
                color: {
                    value: '#ffffff'
                },
                links: {
                    color: '#000000',
                    distance: 150,
                    enable: false,
                    opacity: 0.5,
                    width: 1
                },
                collisions: {
                    enable: true
                },
                move: {
                    direction: 'none',
                    enable: true,
                    outMode: 'bounce',
                    random: false,
                    speed: 6,
                    straight: false
                },
                number: {
                    density: {
                        enable: true,
                        value_area: x
                    },
                    value: 80
                },
                opacity: {
                    value: 0.5
                },
                shape: {
                    type: 'circle'
                },
                size: {
                    random: true,
                    value: 3
                }
            },
            detectRetina: true
        }"
    ></Particles>
</client-only>
</template>

<script>
import Particles from "particles.vue";

export default {
  name: 'particles',

  methods: {
    adjustParticles(){
      this.x = 500;
    }
  },

  data () {
    return {
      x: 500
    }
  },

  mounted() {
    this.adjustParticles();
  }
}
</script>

<style>
#tsparticles {
    position: absolute;
    left: 0;
    top: 56px;
    width: 100%;
    height: calc(100vh - 56px);
}
</style>