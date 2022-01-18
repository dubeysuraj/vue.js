<template>
<div>
  <!-- <img src="./assets/logo.png" alt="" width="100"> -->
  <Home />
  <DataBind />
  <Child v-bind:users="users" />
  </div>
  
</template>

<script>

// import Home from './components/Home.vue';
import Home from './components/Home.vue'
import DataBind from './components/DataBind.vue'
import Child from './components/Child.vue'

export default {
  name: 'App',
  components: {
  
    Home,
    DataBind,
    Child,
  },
    data(){
     return{users: [
         {name: "Suraj", email: "suraj@gmail.com"},
         {name: "charlie", email: "charlie@gmail.com"},
         {name : "Selena", email: "selena@gmail.com"},
         {name : "Ariana", email: "ariana@gmail.com"},
     ]
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
</style>
