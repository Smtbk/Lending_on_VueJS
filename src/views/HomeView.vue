<template>
  <div class="pad65"></div>
  <div class="home">
    <HomePage/>
  </div>
</template>

<script>
import HomePage from '@/components/HomePage.vue'

export default {
  name: 'HomeView',
  components: {
    HomePage
  }
}
</script>

<style scope>
.pad65 {
  padding-top: 65px; 
}
</style>
