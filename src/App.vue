<template>
  <div id="app">
    
    <Tilt :options="this.options">

      <div class="Background">
        <img alt="Vue logo" src="./assets/logo.png">
        <HelloWorld class="pop" msg="Welcome to Your Vue.js App"/>
        
      </div>
    </Tilt>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Tilt from './components/tilt'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Tilt
  },
  data: function(){
    return {
      options: {glare: true}
    }
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

.Background{
  background-color: greenyellow;
}

.pop{
  transform: translateZ(20px)
}
</style>
