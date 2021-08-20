<template>
  <div id="app" class="container mt-5">
    <List></List>
  </div>
</template>

<script>
import List from './components/List.vue'
export default {
  name: 'App',
  components: {
    List
  },

  data: () => ({})
}
</script>

<style>
body {
  background-image: url(../public/backgroundimage.png);
}
</style>
