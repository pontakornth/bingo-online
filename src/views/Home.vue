<template>
  <div class="home">
    <h1 class="heading text-light-color">Bingo Online</h1>
    <div class="menu">
      <router-link to="/host" class="button">Create Room</router-link>
      <router-link to="/bingo" class="button is-secondary">Join Room</router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>

<style lang="stylus">
@import '../assets/style.styl'
@import '../assets/mixins.styl'
.home
  column-centered
  text-align center
  height 100vh
  background darken(primary,20%)
  & .heading
    color darked(#ffffff,10%)

.heading
  font-size 4rem

.menu
  padding 2rem
  margin auto
  display grid
  grid-template-columns repeat(1, 1fr)
  grid-gap 0.5rem

</style>
