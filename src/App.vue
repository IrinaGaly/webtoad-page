<template>
  <div id="app" class="o-main-wrapper">
    <SectionAbout />
  </div>
</template>

<script>
import SectionAbout from './components/SectionAbout.vue'

export default {
  name: 'App',
  components: {
    SectionAbout,
  }
}
</script>

<style lang="scss">
@import './scss/main.scss';
</style>
