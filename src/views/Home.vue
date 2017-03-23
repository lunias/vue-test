<template lang="pug">
section.section
  .box(v-html="msg")
</template>

<script>
function lorem (numParagraphs) {
  var lorem = ''
  for (var i = 0; i < numParagraphs; i++) {
    lorem += '<p>'
    for (var j = 0; j < Math.floor(Math.random() * 100) + 20; j++) {
      lorem += 'lorem ipsum '
    }
    lorem += '</p>'
  }
  return lorem
}

export default {
  data: function () {
    return {
      msg: lorem(20)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>

</style>
