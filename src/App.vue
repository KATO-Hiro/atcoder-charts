<template lang="pug">
.app
  router-view
</template>

<script lang="ts">
import '@/styles/simple-reset.css'
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component({
  components: {},
})
export default class App extends Vue {
  errorCaptured(error: Error) {
    console.log(error)
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=PT+Serif|Poppins|Righteous&display=swap');

:root {
  --black: #202c39;
  --white: #eaeaea;
  --deep-pink: #da4167;
  --royal-blue: #4f7cac;
  --teal: #00a9a5;
  --deep-teal: #008481;
  --clear-teal: #00848238;
  --clear-black: #202c392c;
  --gray: #4f5d75;
}

body {
  color: var(--black);
  background: var(--white);
}

.app {
  height: 100vh;
  font-family: 'Poppins', 'Arial', 'Hiragino Sans', 'ヒラギノ角ゴシック', 'メイリオ', Meiryo,
    sans-serif;
  overflow-y: scroll;
  scroll-behavior: smooth;
}
</style>
