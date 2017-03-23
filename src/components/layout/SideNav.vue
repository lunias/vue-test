<template lang="pug">
aside.menu
  p.menu-label General
  ul.menu-list
    li: a Dashboard
    li: a Customers
  p.menu-label Administration
  ul.menu-list
    li: a Team Settings
    li: a.is-active Manage Your Team
      ul
        li: a Members
        li: a Plugins
        li: a Add a member
    li: a Invitations
</template>

<script>
export default {
  data: function () {
    return {

    }
  },
  methods: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>

</style>
