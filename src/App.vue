<template>
  <div id="app" class="d-flex flex-column h-100">
    <div id="top-container">
      <app-header/>
      <router-view>
    </div>
    <app-footer/>
  </div>
</template>

<script>
import AppHeader from '@/components/global/AppHeader.vue'
import AppFooter from '@/components/global/AppFooter.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: blue;
}

html,body {
  height: 100%
}

#top-container {
  flex: 1 0 auto;
  background: palegoldenrod;
}
</style>
