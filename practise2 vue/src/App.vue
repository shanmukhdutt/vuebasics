<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
<user msg="Welcome to Vue.js App"/> 
<home/>
<!-- <router-link to="/footer">Home</router-link>
<router-link to="/login">Login</router-link>
<router-link to="/profile">Profile</router-link>
<router-view></router-view> -->
</template>

<script>
import User from './components/User.vue';
import Home from './components/Home.vue'
export default {
  name: 'App',
  components:{
    User,
    Home
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
