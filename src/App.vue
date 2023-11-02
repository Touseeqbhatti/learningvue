<template>
<div>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <HomeComponents />
  <ForLoopComponents />
  <TemplateComponents /> -->
    <!-- <HomeComponents data="Touseeq"/> -->
    <!-- <DataBinding /> -->
    <PropsComp v-bind:name="users" />
    

</div>
  
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import HomeComponents from './components/HomeComponents.vue'
// import ForLoopComponents from './components/ForLoopComponents.vue'
// import TemplateComponents from './components/TemplateComponents.vue'
// import DataBinding from './components/DataBinding.vue'
import PropsComp from './components/PropsComp.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // HomeComponents,
    // ForLoopComponents,
    // TemplateComponents,
    // DataBinding,
    PropsComp,
  },
  data(){
    return {users:[
      {name:"touseeq",email:"touseeq@gmail.com"},
      {name:"ali",email:"ali@gmail.com"},
      {name:"ahamd",email:"ahmad@gmail.com"},
      {name:"akmal",email:"akmal@gmail.com"},
    ]}
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
