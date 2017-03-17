<template lang="pug">
#app
  top-nav
  router-view
</template>

<script>
import { TopNav } from 'components/layout'
export default {
  components: {
    TopNav
  }
}
</script>

<style lang="sass">
@import "~bulma"
#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  text-align: center
  color: #2c3e50
  margin-top: 60px
</style>
