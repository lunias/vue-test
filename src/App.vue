<template lang="pug">
#app
  top-nav
  section.section.columns
    .column.is-one-quarter
      side-nav
    .column
      router-view
  page-footer
</template>

<script>
import { TopNav, SideNav, PageFooter } from 'components/layout'
export default {
  components: {
    TopNav,
    SideNav,
    PageFooter
  }
}
</script>

<style lang="sass">
@import "~font-awesome/css/font-awesome.css"
@import "~bulma"
#app
  font-family: 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  color: #2c3e50
</style>
