<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
import 'normalize.css';
import './assets/style.styl';
import Vue from 'vue';

// No class based component is needed here.
export default Vue.extend({
  name: 'App',
});
</script>

<style lang="stylus">
#app
  text-align center
  display flex
  flex-flow column wrap
  justify-content center
  align-items stretch
</style>
