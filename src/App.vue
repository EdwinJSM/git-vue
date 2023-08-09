<template>
   <div class="container">
 <HeaderHeader title="Task Tracker"/>
   </div>
</template>

<script>
import HeaderHeader from './components/HeaderHeader.vue';

export default {
  name: 'App',
  components: {
  HeaderHeader
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ff041d;
  margin-top: 60px;
}
.btn {
  background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>
