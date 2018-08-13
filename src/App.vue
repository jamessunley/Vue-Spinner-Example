<template>
<div class="container">
    <pulse-loader :loading="loading" :color="color" :size="size"></pulse-loader>
    <fade-loader :loading="loading" :color="color" :size="size"></fade-loader>
    <clip-loader :loading="loading" :color="color" :size="size"></clip-loader>
    <beat-loader :loading="loading" :color="color" :size="size"></beat-loader>
    <pacman-loader :loading="loading" :color="color" :size="size"></pacman-loader>
    
  </div>
</template>

<script>
import PulseLoader from 'vue-spinner/src/PulseLoader.vue'
import ClipLoader from 'vue-spinner/src/ClipLoader.vue'
import FadeLoader from 'vue-spinner/src/FadeLoader.vue'
import BeatLoader from 'vue-spinner/src/BeatLoader.vue'
import PacmanLoader from 'vue-spinner/src/PacmanLoader.vue'

export default {
  data () {
    return {
      color: '#cc181e',
      color1: '#5bc0de',
      size: '25px',
      margin: '2px',
      radius: '2px'
    }
  },
  components: {
    PulseLoader,
    ClipLoader,
    FadeLoader,
    BeatLoader,
    PacmanLoader
  }
}
</script>

<style>

</style>
