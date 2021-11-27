<template>
<div>
  <navbar></navbar>
  <div>
    <watchable-card></watchable-card>
  </div>
</div>
</template>

<script>
import navbar from './components/navbar.vue'
import watchableCard from './components/watchableCard.vue'

export default {
  name: 'App',
  components: {
    navbar,
    watchableCard
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
