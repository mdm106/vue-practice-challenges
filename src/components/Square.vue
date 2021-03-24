<template>
  <div :style="style">
  </div>
</template>

<script>

export default {
  name: 'Square',
  props: {
    colour: {
      type: String,
      default: "red"
    },
  },
  computed: {
    style () {
      return 'background-color: ' + this.colour;
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  div {
    width: 200px;
    height: 200px;
    margin: auto;
  }
</style>
