<template>
  <div id="app">
  <Enter v-on:click.native="enterFunc" v-bind:class="{active: enter}"/>
  </div>
</template>

<script>
import Enter from './components/Enter.vue';


export default {
  name: 'app',
  components: {
   Enter,
  
  },
  methods: {
    enterFunc: function(){
      this.enter = !this.enter;
      console.log("click");
    }
  },
  data: function(){
    return {
      enter: false,
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.active {
  display: none;
}
</style>
