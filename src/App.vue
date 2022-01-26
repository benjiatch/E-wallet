<template>
  <div id="app">
    <nav>
      <a @click="currentView = 'home'">Home</a>
      <a @click="currentView = 'addcard'">Add Card</a>
    </nav>
    <Home v-if="currentView == 'home'"/>
    <AddCard v-else-if="currentView == 'addcard'"/>
    
  </div>
</template>

<script>
import Home from './views/Home.vue'
import AddCard from './views/Add-card.vue'

export default {
  components: {Home, AddCard},
  name: 'App',
  data(){return{
    currentView : 'home'
  }}
}

</script>

<style>
.app{
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

a{
  margin: 2rem;
}

</style>
