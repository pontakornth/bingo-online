<template>
    <div class="host bg-primary">
        <div class="host-panel">
            <h1 class="number">1</h1>
            <button class="button is-light-color">Re-roll</button>
        </div>
    </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class Host extends Vue {}
</script>

<style lang="stylus" scoped>
@import "../assets/mixins"
.host
  height 100vh
  display flex
.host-panel
  margin auto
.number
  font-size 3rem
  height 4.5rem
  width 4.5rem
  background darken(#ffffff, 10%)
  border-radius 99999px
  margin 1rem auto
</style>
