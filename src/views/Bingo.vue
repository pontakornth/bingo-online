<template>
    <div class="bingo">
        <h1>Current number is 0</h1>
        <div class="bingo-table">
            <button class="bingo-unit" v-for="i in 25" :key="i">0</button>
        </div>
    </div>
</template>

<script>
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class Bingo extends Vue {}
</script>

<style lang="stylus">
@import "../assets/style.styl"
@import "../assets/mixins.styl"
.bingo
  column-centered()
  background primary
  color light-color
  height 100vh
  justify-content center
  align-items center
.bingo-table
  display grid
  margin auto
  grid-template-columns repeat(5, 50px)
  grid-template-rows repeat(5, 50px)
  justify-items center
  padding 0 4px
  grid-gap 5px
.bingo-unit
    display block
    width 100%
    font-size 2rem
    border-radius 999px
    border none
</style>
