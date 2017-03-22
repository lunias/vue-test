<template lang="pug">
nav.nav.has-shadow

  #nav-left.nav-left
    a.nav-item: img(src="http://bulma.io/images/bulma-logo.png" alt="Bulma logo")

  #nav-center.nav-center
    a.nav-item
      span.icon
        i.fa.fa-github
    a.nav-item
      span.icon
        i.fa.fa-twitter

  span#nav-toggle.nav-toggle(@click="toggleNav" v-bind:class="{ 'is-active': navToggled }")
    span
    span
    span

  #nav-right.nav-right.nav-menu(v-bind:class="{ 'is-active': navToggled }")
    a.nav-item.is-tab.is-active
      span.icon.is-small: i.fa.fa-home
      span Home
    a.nav-item.is-tab Documentation
    a.nav-item.is-tab Blog

    span.nav-item
      a.button
        span.icon: i.fa.fa-twitter
        span Tweet
      a.button.is-primary
        span.icon: i.fa.fa-download
        span Download

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
</style>
