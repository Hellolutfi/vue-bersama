<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <button @click="register = true">Register</button>
    <RegisterUser v-if="register"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import RegisterUser from './components/RegisterUser.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    RegisterUser
  },
  //var register = true
  data(){
    return {
      register: false,
    }
  },
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
