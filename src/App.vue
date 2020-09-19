<template>
  <div id="app">
     <navbar/>
    <router-view/>
  </div>
</template>

<script>
import navbar from './components/navbar.vue'
export default {
  name:"app",
  components:{navbar ,
  } 
}
</script>
<style>

*,*::before,*::afer{
box-sizing: border-box;
}

body{
  margin:0;
  padding:0;
  background:black;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
