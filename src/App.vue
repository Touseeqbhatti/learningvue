<template>
<div>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <HomeComponents />
  <ForLoopComponents />
  <TemplateComponents />
    <!-- <HomeComponents data="Touseeq"/> -->
    

</div>
  
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HomeComponents from './components/HomeComponents.vue'
import ForLoopComponents from './components/ForLoopComponents.vue'
import TemplateComponents from './components/TemplateComponents.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    HomeComponents,
    ForLoopComponents,
    TemplateComponents
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
