<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h1>Hello I M Ronak</h1>
  <!-- <MyComp/> -->
  <!-- <InterPol /> -->
  <!-- <EventClicks /> -->
  <!-- <TwowayBind /> -->
  <!-- <FetchInput/> -->
  <SimpleForm />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import MyComp from './components/MyComp.vue';
// import InterPol from './components/InterPol.vue';
// import EventClicks from './components/EventClicks.vue';
// import TwowayBind from './components/TwowayBind.vue';

// import FetchInput from './components/FetchInput.vue';
import SimpleForm from './components/SimpleForm.vue';
export default {
  name: 'App',
  components: {
    // FetchInput,
    SimpleForm

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
