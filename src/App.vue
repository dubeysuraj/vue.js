<template>
  <div id="app">
    <h1>Form with checkbox and radio button in Vue js</h1>
    <SignUp />
  </div>
  
</template>

<script>
import SignUp from './components/SignUp'

export default {
  name: 'App',
  components: {
    SignUp,
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
