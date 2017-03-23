<template lang="pug">
section.hero.is-primary.is-medium
  .hero-head
    header.nav
      .container
        .nav-left
          a.nav-item: img(src="http://bulma.io/images/bulma-type-white.png" alt="Bulma logo")
        .nav-toggle(@click="toggleNav" v-bind:class="{ 'is-active': navToggled }")
          span
          span
          span
        .nav-right.nav-menu(v-bind:class="{ 'is-active': navToggled }")
          a.nav-item.is-active Home
          a.nav-item Examples
          a.nav-item Documentation

  .hero-body
    .container.has-text-centered
      h1.title Title
      h2.subtitle Subtitle

  .hero-foot
    nav.tabs.is-boxed.has-shadow
      .container
        ul
          li.is-active: a Overview
          li: a Modifiers
          li: a Grid
          li: a Components
</template>

<script>
export default {
  data: function () {
    return {
      navToggled: false
    }
  },
  methods: {
    toggleNav: function () {
      this.navToggled = !this.navToggled
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
h1
  font-weight: normal
.nav
  position: fixed
  top: 0
  left: 0
  right: 0
  background-color: #00d1b2
</style>
